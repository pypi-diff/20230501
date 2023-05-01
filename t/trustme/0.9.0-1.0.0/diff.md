# Comparing `tmp/trustme-0.9.0.tar.gz` & `tmp/trustme-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trustme-0.9.0.tar", last modified: Thu Aug 12 20:04:30 2021, max compression
+gzip compressed data, was "trustme-1.0.0.tar", last modified: Mon May  1 06:16:17 2023, max compression
```

## Comparing `trustme-0.9.0.tar` & `trustme-1.0.0.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2021-08-12 20:04:30.397482 trustme-0.9.0/
--rw-r--r--   0 quentin    (501) staff       (20)      118 2019-12-19 14:04:58.000000 trustme-0.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 quentin    (501) staff       (20)      185 2019-12-19 14:04:58.000000 trustme-0.9.0/LICENSE
--rw-r--r--   0 quentin    (501) staff       (20)    11358 2019-12-19 14:04:58.000000 trustme-0.9.0/LICENSE.APACHE2
--rw-r--r--   0 quentin    (501) staff       (20)     1046 2019-12-19 14:04:58.000000 trustme-0.9.0/LICENSE.MIT
--rw-r--r--   0 quentin    (501) staff       (20)      180 2019-12-19 14:04:58.000000 trustme-0.9.0/MANIFEST.in
--rw-r--r--   0 quentin    (501) staff       (20)     6641 2021-08-12 20:04:30.397959 trustme-0.9.0/PKG-INFO
--rw-r--r--   0 quentin    (501) staff       (20)     4400 2021-03-16 19:25:07.000000 trustme-0.9.0/README.rst
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2021-08-12 20:04:30.370821 trustme-0.9.0/docs/
--rw-r--r--   0 quentin    (501) staff       (20)      611 2019-12-19 14:04:58.000000 trustme-0.9.0/docs/Makefile
--rw-r--r--   0 quentin    (501) staff       (20)      809 2019-12-19 14:04:58.000000 trustme-0.9.0/docs/make.bat
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2021-08-12 20:04:30.374997 trustme-0.9.0/docs/source/
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2021-08-12 20:04:30.376433 trustme-0.9.0/docs/source/_static/
--rw-r--r--   0 quentin    (501) staff       (20)        0 2019-12-19 14:04:58.000000 trustme-0.9.0/docs/source/_static/.gitkeep
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2021-08-12 20:04:30.377364 trustme-0.9.0/docs/source/_templates/
--rw-r--r--   0 quentin    (501) staff       (20)      212 2019-12-19 14:04:58.000000 trustme-0.9.0/docs/source/_templates/need-help.html
--rw-r--r--   0 quentin    (501) staff       (20)     5305 2019-12-19 14:04:58.000000 trustme-0.9.0/docs/source/conf.py
--rw-r--r--   0 quentin    (501) staff       (20)     8376 2021-08-12 19:59:09.000000 trustme-0.9.0/docs/source/index.rst
--rw-r--r--   0 quentin    (501) staff       (20)     2359 2019-12-19 14:04:58.000000 trustme-0.9.0/docs/source/trustme-trio-example.py
--rw-r--r--   0 quentin    (501) staff       (20)     1455 2021-08-12 19:58:05.000000 trustme-0.9.0/pyproject.toml
--rw-r--r--   0 quentin    (501) staff       (20)       67 2021-08-12 20:04:30.399417 trustme-0.9.0/setup.cfg
--rw-r--r--   0 quentin    (501) staff       (20)     1706 2021-08-12 19:58:05.000000 trustme-0.9.0/setup.py
--rw-r--r--   0 quentin    (501) staff       (20)     1952 2021-06-08 17:58:20.000000 trustme-0.9.0/test-requirements.txt
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2021-08-12 20:04:30.380464 trustme-0.9.0/tests/
--rw-r--r--   0 quentin    (501) staff       (20)     3247 2021-08-12 19:58:05.000000 trustme-0.9.0/tests/test_cli.py
--rw-r--r--   0 quentin    (501) staff       (20)    17669 2021-08-12 19:58:05.000000 trustme-0.9.0/tests/test_trustme.py
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2021-08-12 20:04:30.387938 trustme-0.9.0/trustme/
--rw-r--r--   0 quentin    (501) staff       (20)    21005 2021-08-12 19:58:05.000000 trustme-0.9.0/trustme/__init__.py
--rw-r--r--   0 quentin    (501) staff       (20)       56 2021-02-10 06:22:45.000000 trustme-0.9.0/trustme/__main__.py
--rw-r--r--   0 quentin    (501) staff       (20)     3092 2021-08-12 19:58:05.000000 trustme-0.9.0/trustme/_cli.py
--rw-r--r--   0 quentin    (501) staff       (20)       22 2021-08-12 19:59:03.000000 trustme-0.9.0/trustme/_version.py
--rw-r--r--   0 quentin    (501) staff       (20)        0 2021-08-12 19:58:05.000000 trustme-0.9.0/trustme/py.typed
-drwxr-xr-x   0 quentin    (501) staff       (20)        0 2021-08-12 20:04:30.396480 trustme-0.9.0/trustme.egg-info/
--rw-r--r--   0 quentin    (501) staff       (20)     6641 2021-08-12 20:04:29.000000 trustme-0.9.0/trustme.egg-info/PKG-INFO
--rw-r--r--   0 quentin    (501) staff       (20)      593 2021-08-12 20:04:29.000000 trustme-0.9.0/trustme.egg-info/SOURCES.txt
--rw-r--r--   0 quentin    (501) staff       (20)        1 2021-08-12 20:04:29.000000 trustme-0.9.0/trustme.egg-info/dependency_links.txt
--rw-r--r--   0 quentin    (501) staff       (20)       55 2021-08-12 20:04:29.000000 trustme-0.9.0/trustme.egg-info/requires.txt
--rw-r--r--   0 quentin    (501) staff       (20)        8 2021-08-12 20:04:29.000000 trustme-0.9.0/trustme.egg-info/top_level.txt
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.662828 trustme-1.0.0/
+-rw-r--r--   0 q         (1000) q         (1000)      118 2021-10-04 05:59:43.000000 trustme-1.0.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 q         (1000) q         (1000)      185 2021-10-04 05:59:43.000000 trustme-1.0.0/LICENSE
+-rw-r--r--   0 q         (1000) q         (1000)    11358 2021-10-04 05:59:43.000000 trustme-1.0.0/LICENSE.APACHE2
+-rw-r--r--   0 q         (1000) q         (1000)     1046 2021-10-04 05:59:43.000000 trustme-1.0.0/LICENSE.MIT
+-rw-r--r--   0 q         (1000) q         (1000)      180 2021-10-04 05:59:43.000000 trustme-1.0.0/MANIFEST.in
+-rw-r--r--   0 q         (1000) q         (1000)     5581 2023-05-01 06:16:17.661828 trustme-1.0.0/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)     4385 2022-06-07 05:49:38.000000 trustme-1.0.0/README.rst
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.659828 trustme-1.0.0/docs/
+-rw-r--r--   0 q         (1000) q         (1000)      611 2021-10-04 05:59:43.000000 trustme-1.0.0/docs/Makefile
+-rw-r--r--   0 q         (1000) q         (1000)      809 2021-10-04 05:59:43.000000 trustme-1.0.0/docs/make.bat
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.659828 trustme-1.0.0/docs/source/
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.659828 trustme-1.0.0/docs/source/_static/
+-rw-r--r--   0 q         (1000) q         (1000)        0 2021-10-04 05:59:43.000000 trustme-1.0.0/docs/source/_static/.gitkeep
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.659828 trustme-1.0.0/docs/source/_templates/
+-rw-r--r--   0 q         (1000) q         (1000)      212 2021-10-04 05:59:43.000000 trustme-1.0.0/docs/source/_templates/need-help.html
+-rw-r--r--   0 q         (1000) q         (1000)     5333 2022-06-07 05:49:38.000000 trustme-1.0.0/docs/source/conf.py
+-rw-r--r--   0 q         (1000) q         (1000)     9184 2023-05-01 06:09:23.000000 trustme-1.0.0/docs/source/index.rst
+-rw-r--r--   0 q         (1000) q         (1000)     2357 2022-06-07 05:49:38.000000 trustme-1.0.0/docs/source/trustme-trio-example.py
+-rw-r--r--   0 q         (1000) q         (1000)     1605 2023-04-24 05:34:31.000000 trustme-1.0.0/pyproject.toml
+-rw-r--r--   0 q         (1000) q         (1000)       38 2023-05-01 06:16:17.662828 trustme-1.0.0/setup.cfg
+-rw-r--r--   0 q         (1000) q         (1000)     1538 2023-05-01 06:01:58.000000 trustme-1.0.0/setup.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.657828 trustme-1.0.0/src/
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.660828 trustme-1.0.0/src/trustme/
+-rw-r--r--   0 q         (1000) q         (1000)    19643 2023-04-24 05:34:31.000000 trustme-1.0.0/src/trustme/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)       31 2023-04-24 05:34:31.000000 trustme-1.0.0/src/trustme/__main__.py
+-rw-r--r--   0 q         (1000) q         (1000)     3072 2023-04-24 05:34:31.000000 trustme-1.0.0/src/trustme/_cli.py
+-rw-r--r--   0 q         (1000) q         (1000)       22 2023-05-01 06:01:58.000000 trustme-1.0.0/src/trustme/_version.py
+-rw-r--r--   0 q         (1000) q         (1000)        0 2023-04-24 05:34:31.000000 trustme-1.0.0/src/trustme/py.typed
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.661828 trustme-1.0.0/src/trustme.egg-info/
+-rw-r--r--   0 q         (1000) q         (1000)     5581 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)      623 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/SOURCES.txt
+-rw-r--r--   0 q         (1000) q         (1000)        1 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/dependency_links.txt
+-rw-r--r--   0 q         (1000) q         (1000)       28 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/requires.txt
+-rw-r--r--   0 q         (1000) q         (1000)        8 2023-05-01 06:16:17.000000 trustme-1.0.0/src/trustme.egg-info/top_level.txt
+-rw-r--r--   0 q         (1000) q         (1000)      863 2023-04-24 05:35:28.000000 trustme-1.0.0/test-requirements.txt
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 06:16:17.661828 trustme-1.0.0/tests/
+-rw-r--r--   0 q         (1000) q         (1000)     3253 2023-04-17 10:20:58.000000 trustme-1.0.0/tests/test_cli.py
+-rw-r--r--   0 q         (1000) q         (1000)    16905 2023-04-24 05:34:31.000000 trustme-1.0.0/tests/test_trustme.py
```

### Comparing `trustme-0.9.0/LICENSE.APACHE2` & `trustme-1.0.0/LICENSE.APACHE2`

 * *Files identical despite different names*

### Comparing `trustme-0.9.0/LICENSE.MIT` & `trustme-1.0.0/LICENSE.MIT`

 * *Files identical despite different names*

### Comparing `trustme-0.9.0/PKG-INFO` & `trustme-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,162 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: trustme
-Version: 0.9.0
+Version: 1.0.0
 Summary: #1 quality TLS certs while you wait, for the discerning tester
 Home-page: https://github.com/python-trio/trustme
 Author: Nathaniel J. Smith
 Author-email: njs@pobox.com
-License: MIT -or- Apache License 2.0
-Description: .. note that this README gets 'include'ed into the main documentation
-        
-        ==============================================
-         trustme: #1 quality TLS certs while you wait
-        ==============================================
-        
-        .. image:: https://vignette2.wikia.nocookie.net/jadensadventures/images/1/1e/Kaa%27s_hypnotic_eyes.jpg/revision/latest?cb=20140310173415
-           :width: 200px
-           :align: right
-        
-        You wrote a cool network client or server. It encrypts connections
-        using `TLS
-        <https://en.wikipedia.org/wiki/Transport_Layer_Security>`__. Your test
-        suite needs to make TLS connections to itself.
-        
-        Uh oh. Your test suite *probably* doesn't have a valid TLS
-        certificate. Now what?
-        
-        ``trustme`` is a tiny Python package that does one thing: it gives you
-        a `fake <https://martinfowler.com/bliki/TestDouble.html>`__
-        certificate authority (CA) that you can use to generate fake TLS certs
-        to use in your tests. Well, technically they're real certs, they're
-        just signed by your CA, which nobody trusts. But you can trust
-        it. Trust me.
-        
-        
-        Vital statistics
-        ================
-        
-        **Install:** ``pip install -U trustme``
-        
-        **Documentation:** https://trustme.readthedocs.io
-        
-        **Bug tracker and source code:** https://github.com/python-trio/trustme
-        
-        **Tested on:** Python 2.7 and Python 3.5+, CPython and PyPy
-        
-        **License:** MIT or Apache 2, your choice.
-        
-        **Code of conduct:** Contributors are requested to follow our `code of
-        conduct
-        <https://github.com/python-trio/trustme/blob/master/CODE_OF_CONDUCT.md>`__
-        in all project spaces.
-        
-        
-        Cheat sheet
-        ===========
-        
-        Programmatic usage:
-        
-        .. code-block:: python
-        
-           import trustme
-        
-           # ----- Creating certs -----
-        
-           # Look, you just created your certificate authority!
-           ca = trustme.CA()
-        
-           # And now you issued a cert signed by this fake CA
-           # https://en.wikipedia.org/wiki/Example.org
-           server_cert = ca.issue_cert(u"test-host.example.org")
-        
-           # That's it!
-        
-           # ----- Using your shiny new certs -----
-        
-           # You can configure SSL context objects to trust this CA:
-           ca.configure_trust(ssl_context)
-           # Or configure them to present the server certificate
-           server_cert.configure_cert(ssl_context)
-           # You can use standard library or PyOpenSSL context objects here,
-           # trustme is happy either way.
-        
-           # ----- or -----
-                        
-           # Save the PEM-encoded data to a file to use in non-Python test
-           # suites:
-           ca.cert_pem.write_to_path("ca.pem")
-           server_cert.private_key_and_cert_chain_pem.write_to_path("server.pem")
-           
-           # ----- or -----
-                        
-           # Put the PEM-encoded data in a temporary file, for libraries that
-           # insist on that:
-           with ca.cert_pem.tempfile() as ca_temp_path:
-               requests.get("https://...", verify=ca_temp_path)
-        
-        Command line usage:
-        
-        .. code-block:: console
-        
-           $ # Certs may be generated from anywhere. Here's where we are:
-           $ pwd
-           /tmp
-           $ # ----- Creating certs -----
-           $ python -m trustme
-           Generated a certificate for 'localhost', '127.0.0.1', '::1'
-           Configure your server to use the following files:
-             cert=/tmp/server.pem
-             key=/tmp/server.key
-           Configure your client to use the following files:
-             cert=/tmp/client.pem
-           $ # ----- Using certs -----
-           $ gunicorn --keyfile server.key --certfile server.pem app:app
-           $ curl --cacert client.pem https://localhost:8000/
-           Hello, world!
-        
-        
-        FAQ
-        ===
-        
-        **Should I use these certs for anything real?** Certainly not.
-        
-        **Why not just use self-signed certificates?** These are more
-        realistic. You don't have to disable your certificate validation code
-        in your test suite, which is good because you want to test what you
-        run in production, and you would *never* disable your certificate
-        validation code in production, right? Plus, they're just as easy to
-        work with. Actually easier, in many cases.
-        
-        **What if I want to test how my code handles some bizarre TLS
-        configuration?** We think trustme hits a sweet spot of ease-of-use
-        and generality as it is. The defaults are carefully chosen to work
-        on all major operating systems and be as fast as possible. We don't
-        want to turn trustme into a second-rate re-export of everything in
-        `cryptography <https://cryptography.io>`__. If you have more complex
-        needs, consider using them directly, possibly starting from the
-        trustme code.
-        
-        **Will you automate installing CA cert into system trust store?** No.
-        `mkcert <https://github.com/FiloSottile/mkcert>`__ already does this
-        well, and we would not have anything to add.
-        
-Platform: UNKNOWN
+License: MIT OR Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
+License-File: LICENSE
+License-File: LICENSE.APACHE2
+License-File: LICENSE.MIT
+
+.. note that this README gets 'include'ed into the main documentation
+
+==============================================
+ trustme: #1 quality TLS certs while you wait
+==============================================
+
+.. image:: https://vignette2.wikia.nocookie.net/jadensadventures/images/1/1e/Kaa%27s_hypnotic_eyes.jpg/revision/latest?cb=20140310173415
+   :width: 200px
+   :align: right
+
+You wrote a cool network client or server. It encrypts connections
+using `TLS
+<https://en.wikipedia.org/wiki/Transport_Layer_Security>`__. Your test
+suite needs to make TLS connections to itself.
+
+Uh oh. Your test suite *probably* doesn't have a valid TLS
+certificate. Now what?
+
+``trustme`` is a tiny Python package that does one thing: it gives you
+a `fake <https://martinfowler.com/bliki/TestDouble.html>`__
+certificate authority (CA) that you can use to generate fake TLS certs
+to use in your tests. Well, technically they're real certs, they're
+just signed by your CA, which nobody trusts. But you can trust
+it. Trust me.
+
+
+Vital statistics
+================
+
+**Install:** ``pip install -U trustme``
+
+**Documentation:** https://trustme.readthedocs.io
+
+**Bug tracker and source code:** https://github.com/python-trio/trustme
+
+**Tested on:** Python 3.7+, CPython and PyPy
+
+**License:** MIT or Apache 2, your choice.
+
+**Code of conduct:** Contributors are requested to follow our `code of
+conduct
+<https://github.com/python-trio/trustme/blob/master/CODE_OF_CONDUCT.md>`__
+in all project spaces.
+
+
+Cheat sheet
+===========
+
+Programmatic usage:
+
+.. code-block:: python
+
+   import trustme
+
+   # ----- Creating certs -----
+
+   # Look, you just created your certificate authority!
+   ca = trustme.CA()
+
+   # And now you issued a cert signed by this fake CA
+   # https://en.wikipedia.org/wiki/Example.org
+   server_cert = ca.issue_cert(u"test-host.example.org")
+
+   # That's it!
+
+   # ----- Using your shiny new certs -----
+
+   # You can configure SSL context objects to trust this CA:
+   ca.configure_trust(ssl_context)
+   # Or configure them to present the server certificate
+   server_cert.configure_cert(ssl_context)
+   # You can use standard library or PyOpenSSL context objects here,
+   # trustme is happy either way.
+
+   # ----- or -----
+                
+   # Save the PEM-encoded data to a file to use in non-Python test
+   # suites:
+   ca.cert_pem.write_to_path("ca.pem")
+   server_cert.private_key_and_cert_chain_pem.write_to_path("server.pem")
+   
+   # ----- or -----
+                
+   # Put the PEM-encoded data in a temporary file, for libraries that
+   # insist on that:
+   with ca.cert_pem.tempfile() as ca_temp_path:
+       requests.get("https://...", verify=ca_temp_path)
+
+Command line usage:
+
+.. code-block:: console
+
+   $ # Certs may be generated from anywhere. Here's where we are:
+   $ pwd
+   /tmp
+   $ # ----- Creating certs -----
+   $ python -m trustme
+   Generated a certificate for 'localhost', '127.0.0.1', '::1'
+   Configure your server to use the following files:
+     cert=/tmp/server.pem
+     key=/tmp/server.key
+   Configure your client to use the following files:
+     cert=/tmp/client.pem
+   $ # ----- Using certs -----
+   $ gunicorn --keyfile server.key --certfile server.pem app:app
+   $ curl --cacert client.pem https://localhost:8000/
+   Hello, world!
+
+
+FAQ
+===
+
+**Should I use these certs for anything real?** Certainly not.
+
+**Why not just use self-signed certificates?** These are more
+realistic. You don't have to disable your certificate validation code
+in your test suite, which is good because you want to test what you
+run in production, and you would *never* disable your certificate
+validation code in production, right? Plus, they're just as easy to
+work with. Actually easier, in many cases.
+
+**What if I want to test how my code handles some bizarre TLS
+configuration?** We think trustme hits a sweet spot of ease-of-use
+and generality as it is. The defaults are carefully chosen to work
+on all major operating systems and be as fast as possible. We don't
+want to turn trustme into a second-rate re-export of everything in
+`cryptography <https://cryptography.io>`__. If you have more complex
+needs, consider using them directly, possibly starting from the
+trustme code.
+
+**Will you automate installing CA cert into system trust store?** No.
+`mkcert <https://github.com/FiloSottile/mkcert>`__ already does this
+well, and we would not have anything to add.
```

### Comparing `trustme-0.9.0/README.rst` & `trustme-1.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 **Install:** ``pip install -U trustme``
 
 **Documentation:** https://trustme.readthedocs.io
 
 **Bug tracker and source code:** https://github.com/python-trio/trustme
 
-**Tested on:** Python 2.7 and Python 3.5+, CPython and PyPy
+**Tested on:** Python 3.7+, CPython and PyPy
 
 **License:** MIT or Apache 2, your choice.
 
 **Code of conduct:** Contributors are requested to follow our `code of
 conduct
 <https://github.com/python-trio/trustme/blob/master/CODE_OF_CONDUCT.md>`__
 in all project spaces.
```

### Comparing `trustme-0.9.0/docs/Makefile` & `trustme-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `trustme-0.9.0/docs/make.bat` & `trustme-1.0.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `trustme-0.9.0/docs/source/conf.py` & `trustme-1.0.0/docs/source/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 #
 # trustme documentation build configuration file, created by
 # sphinx-quickstart on Tue Jul 18 01:46:01 2017.
 #
 # This file is execfile()d with the current directory set to its
 # containing dir.
 #
@@ -45,15 +44,16 @@
     #'sphinx.ext.viewcode',
     'sphinx.ext.napoleon',
     'sphinxcontrib_trio',
 ]
 
 intersphinx_mapping = {
     "python": ('https://docs.python.org/3', None),
-    "pyopenssl": ('https://www.pyopenssl.org/en/stable/', None),
+    # https://github.com/pyca/pyopenssl/issues/1046
+    "pyopenssl": ('https://www.pyopenssl.org/en/20.0.1/', None),
     "trio": ('https://trio.readthedocs.io/en/latest/', None),
 }
 
 autodoc_member_order = "bysource"
 
 # Tell sphinx to treat bare backticks like `foo` as :py:obj:`foo`
 default_role = 'py:obj'
@@ -86,15 +86,15 @@
 release = version
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = []
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `trustme-0.9.0/docs/source/index.rst` & `trustme-1.0.0/docs/source/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 ====================
 
 Here's a fully working example you can run to see how :mod:`trustme`
 works. It demonstrates a simple TLS server and client that connect to
 each other using :mod:`trustme`\-generated certs.
 
 This example requires `Trio <https://trio.readthedocs.io>`__ (``pip
-install -U trio``) and Python 3.5+. Note that while :mod:`trustme` is
+install -U trio``) and Python 3.7+. Note that while :mod:`trustme` is
 maintained by the Trio project, :mod:`trustme` is happy to work with
-any networking library, and also supports Python 2.
+any networking library.
 
 The key lines are the calls to :meth:`~CA.configure_trust`,
 :meth:`~LeafCert.configure_cert` – try commenting them out one at a
 time to see what happens! Also notice that the hostname
 ``test-host.example.org`` appears twice – try changing one of the
 strings so that the two copies no longer match, and see what happens
 then!
@@ -109,20 +109,40 @@
    .. automethod:: bytes
 
    .. automethod:: tempfile
       :with: path
 
    .. automethod:: write_to_path
 
+.. autoclass:: KeyType
+   :members: RSA, ECDSA
+   :undoc-members:
 
 Change history
 ==============
 
 .. towncrier release notes start
 
+Trustme 1.0.0 (2023-04-24)
+------------------------------
+
+Features
+~~~~~~~~
+
+- Support for ECDSA keys in certificates and use them by default. The type of key used for certificates can be controlled by the ``key_type`` parameter on the multiple methods that generate certificates. ECDSA certificates as they can be generated significantly faster. (`#559 <https://github.com/python-trio/trustme/issues/559>`__)
+- Support for Python 3.10 and 3.11 (`#372 <https://github.com/python-trio/trustme/pull/372>`__, `574 <https://github.com/python-trio/trustme/pull/574>`__)
+
+
+
+Deprecations and Removals
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+- Remove support for Python 2. trustme now requires Python>=3.7 (CPython or PyPy). (`#346 <https://github.com/python-trio/trustme/issues/346>`__)
+
+
 Trustme 0.9.0 (2021-08-12)
 --------------------------
 
 Features
 ~~~~~~~~
 
 - The package is now type annotated. If you use mypy on code which uses ``trustme``, you should be able to remove any exclusions. (`#339 <https://github.com/python-trio/trustme/issues/339>`__)
```

### Comparing `trustme-0.9.0/docs/source/trustme-trio-example.py` & `trustme-1.0.0/docs/source/trustme-trio-example.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import trustme
 import trio
 import ssl
 
 # Create our fake certificates
 ca = trustme.CA()
-server_cert = ca.issue_cert(u"test-host.example.org")
-client_cert = ca.issue_cert(u"client@example.org")
+server_cert = ca.issue_cert("test-host.example.org")
+client_cert = ca.issue_cert("client@example.org")
 
 
 async def demo_server(server_raw_stream):
     server_ssl_context = ssl.create_default_context(
         ssl.Purpose.CLIENT_AUTH)
 
     # Set up the server's SSLContext to use our fake server cert
```

### Comparing `trustme-0.9.0/pyproject.toml` & `trustme-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #   (or towncrier --draft)
 # - Make sure to use a version with the PRs mentioned below merged.
 #   You probably want https://github.com/hawkowl/towncrier/pull/69 too.
 #   Right now on my laptop it's
 #     PYTHONPATH=~/src/towncrier/src ~/src/towncrier/bin/towncrier
 #   with the merge-64-66-69 branch checked out.
 package = "trustme"
+package_dir = "src"
 filename = "docs/source/index.rst"
 directory = "newsfragments"
 # Requires https://github.com/hawkowl/towncrier/pull/64
 underlines = ["-", "~", "^"]
 # Requires https://github.com/hawkowl/towncrier/pull/66
 issue_format = "`#{issue} <https://github.com/python-trio/trustme/issues/{issue}>`__"
 
@@ -30,13 +31,23 @@
 no_implicit_reexport = true
 show_error_codes = true
 strict_equality = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
-# Some ignores are only for python2/python3.
-# warn_unused_ignores = true
+warn_unused_ignores = true
 
-[[tool.mypy.overrides]]
-module = "pytest"
-ignore_missing_imports = true
+[tool.coverage.run]
+branch = true
+omit = ["*/setup.py"]
+source = ["trustme"]
+
+[tool.coverage.paths]
+source = ["trustme", "*/trustme", "*\\trustme"]
+
+[tool.coverage.setup]
+precision = 1
+exclude_lines = [
+  "pragma: no cover",
+  "if TYPE_CHECKING:"
+]
```

### Comparing `trustme-0.9.0/setup.py` & `trustme-1.0.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 from setuptools import setup, find_packages
 
 # defines __version__
-exec(open("trustme/_version.py").read())
+exec(open("src/trustme/_version.py").read())
 
 setup(
     name="trustme",
     version=__version__,
     description=
       "#1 quality TLS certs while you wait, for the discerning tester",
     long_description=open("README.rst").read(),
     author="Nathaniel J. Smith",
     author_email="njs@pobox.com",
-    license="MIT -or- Apache License 2.0",
-    packages=find_packages(),
+    license="MIT OR Apache-2.0",
+    packages=find_packages(where="src"),
     package_data={
         'trustme': ['py.typed'],
     },
+    package_dir={'': 'src'},
     url="https://github.com/python-trio/trustme",
+    python_requires=">=3.7",
     install_requires=[
-        "cryptography",
-        # cryptography depends on both of these too, so we should declare our
-        # dependencies to be accurate, but they don't actually cost anything:
-        "idna",
-        "ipaddress; python_version < '3.3'",
+        "cryptography>=3.1",
+        "idna>=2.0",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: System :: Networking",
         "Topic :: Security :: Cryptography",
         "Topic :: Software Development :: Testing",
     ])
```

### Comparing `trustme-0.9.0/test-requirements.txt` & `trustme-1.0.0/test-requirements.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,97 +1,41 @@
 #
-# This file is autogenerated by pip-compile
-# To update, run:
+# This file is autogenerated by pip-compile with Python 3.8
+# by the following command:
 #
 #    pip-compile test-requirements.in
 #
-atomicwrites==1.4.0
-    # via pytest
-attrs==21.2.0
-    # via
-    #   pytest
-    #   service-identity
-backports.functools-lru-cache==1.6.4
-    # via wcwidth
-cffi==1.14.5
+attrs==23.1.0
+    # via service-identity
+cffi==1.15.1
     # via cryptography
-configparser==4.0.2
-    # via importlib-metadata
-contextlib2==0.6.0.post1
-    # via
-    #   importlib-metadata
-    #   zipp
-coverage==5.5
-    # via pytest-cov
-cryptography==2.9.2
+coverage[toml]==7.2.3
+    # via -r test-requirements.in
+cryptography==40.0.2
     # via
     #   -r test-requirements.in
     #   pyopenssl
     #   service-identity
-enum34==1.1.10
-    # via cryptography
-funcsigs==1.0.2
-    # via pytest
-futures==3.1.1 ; python_version < "3.2"
-    # via -r test-requirements.in
-idna==2.10 ; python_version < "3"
+idna==3.4
     # via -r test-requirements.in
-importlib-metadata==2.0.0
-    # via
-    #   pluggy
-    #   pytest
-ipaddress==1.0.23
-    # via
-    #   cryptography
-    #   service-identity
-more-itertools==5.0.0 ; python_version < "3"
-    # via
-    #   -r test-requirements.in
-    #   pytest
-packaging==20.9
+iniconfig==2.0.0
     # via pytest
-pathlib2==2.3.5
-    # via
-    #   importlib-metadata
-    #   pytest
-pluggy==0.13.1
+packaging==23.1
     # via pytest
-py==1.10.0
+pluggy==1.0.0
     # via pytest
-pyasn1-modules==0.2.8
-    # via service-identity
 pyasn1==0.4.8
     # via
     #   pyasn1-modules
     #   service-identity
-pycparser==2.20
+pyasn1-modules==0.3.0
+    # via service-identity
+pycparser==2.21
     # via cffi
-pyopenssl==19.1.0
+pyopenssl==23.1.1
     # via -r test-requirements.in
-pyparsing==2.4.7
-    # via packaging
-pytest-cov==2.12.1
+pytest==7.3.1
     # via -r test-requirements.in
-pytest==4.6.3
-    # via
-    #   -r test-requirements.in
-    #   pytest-cov
-scandir==1.10.0
-    # via pathlib2
 service-identity==21.1.0
     # via -r test-requirements.in
 six==1.16.0
-    # via
-    #   cryptography
-    #   more-itertools
-    #   pathlib2
-    #   pyopenssl
-    #   pytest
-    #   service-identity
-toml==0.10.2
-    # via pytest-cov
-wcwidth==0.2.5
-    # via pytest
-zipp==1.2.0 ; python_version < "3"
-    # via
-    #   -r test-requirements.in
-    #   importlib-metadata
+    # via service-identity
```

### Comparing `trustme-0.9.0/tests/test_trustme.py` & `trustme-1.0.0/tests/test_trustme.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,62 +1,52 @@
-# -*- coding: utf-8 -*-
-
-import py
 import pytest
 
 import sys
 import ssl
 import socket
-import threading
 import datetime
-from concurrent.futures import ThreadPoolExecutor  # type: ignore[import]
-
+from concurrent.futures import ThreadPoolExecutor
 from ipaddress import IPv4Address, IPv6Address, IPv4Network, IPv6Network
+from pathlib import Path
+from typing import Callable, Optional, Union
 
 from cryptography import x509
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.serialization import (
     Encoding, PublicFormat, load_pem_private_key)
 
 import OpenSSL.SSL
 import service_identity.pyopenssl  # type: ignore[import]
 
 import trustme
-from trustme import CA, LeafCert
+from trustme import CA, LeafCert, KeyType
 
-TYPE_CHECKING = False
-if TYPE_CHECKING:  # pragma: no cover
-    from typing import Callable, Optional, Text, Union
 
-    SslSocket = Union[ssl.SSLSocket, OpenSSL.SSL.Connection]
+SslSocket = Union[ssl.SSLSocket, OpenSSL.SSL.Connection]
 
 
-def _path_length(ca_cert):
-    # type: (x509.Certificate) -> Optional[int]
+def _path_length(ca_cert: x509.Certificate) -> Optional[int]:
     bc = ca_cert.extensions.get_extension_for_class(x509.BasicConstraints)
     return bc.value.path_length
 
 
-def assert_is_ca(ca_cert):
-    # type: (x509.Certificate) -> None
+def assert_is_ca(ca_cert: x509.Certificate) -> None:
     bc = ca_cert.extensions.get_extension_for_class(x509.BasicConstraints)
     assert bc.value.ca is True
     assert bc.critical is True
 
     ku = ca_cert.extensions.get_extension_for_class(x509.KeyUsage)
     assert ku.value.key_cert_sign is True
     assert ku.value.crl_sign is True
     assert ku.critical is True
 
     with pytest.raises(x509.ExtensionNotFound):
         ca_cert.extensions.get_extension_for_class(x509.ExtendedKeyUsage)
 
 
-def assert_is_leaf(leaf_cert):
-    # type: (x509.Certificate) -> None
+def assert_is_leaf(leaf_cert: x509.Certificate) -> None:
     bc = leaf_cert.extensions.get_extension_for_class(x509.BasicConstraints)
     assert bc.value.ca is False
     assert bc.critical is True
 
     ku = leaf_cert.extensions.get_extension_for_class(x509.KeyUsage)
     assert ku.value.digital_signature is True
     assert ku.value.key_encipherment is True
@@ -69,262 +59,247 @@
         x509.oid.ExtendedKeyUsageOID.CLIENT_AUTH,
         x509.oid.ExtendedKeyUsageOID.SERVER_AUTH,
         x509.oid.ExtendedKeyUsageOID.CODE_SIGNING
     ])
     assert eku.critical is True
 
 
-def test_basics():
-    # type: () -> None
-    ca = CA()
+@pytest.mark.parametrize(
+    "key_type,expected_key_header", [(KeyType.RSA, b"RSA"), (KeyType.ECDSA, b"EC")]
+)
+def test_basics(key_type: KeyType, expected_key_header: bytes) -> None:
+    ca = CA(key_type=key_type)
 
     today = datetime.datetime.today()
 
-    assert b"BEGIN RSA PRIVATE KEY" in ca.private_key_pem.bytes()
+    assert (
+        b"BEGIN " + expected_key_header + b" PRIVATE KEY" in ca.private_key_pem.bytes()
+    )
     assert b"BEGIN CERTIFICATE" in ca.cert_pem.bytes()
 
-    private_key = load_pem_private_key(
-        ca.private_key_pem.bytes(), password=None, backend=default_backend())
+    private_key = load_pem_private_key(ca.private_key_pem.bytes(), password=None)
 
-    ca_cert = x509.load_pem_x509_certificate(
-        ca.cert_pem.bytes(), default_backend())
+    ca_cert = x509.load_pem_x509_certificate(ca.cert_pem.bytes())
     assert ca_cert.not_valid_before <= today <= ca_cert.not_valid_after
 
     public_key1 = private_key.public_key().public_bytes(
-        Encoding.PEM, PublicFormat.PKCS1)
+        Encoding.PEM, PublicFormat.SubjectPublicKeyInfo
+    )
     public_key2 = ca_cert.public_key().public_bytes(
-        Encoding.PEM, PublicFormat.PKCS1)
+        Encoding.PEM, PublicFormat.SubjectPublicKeyInfo
+    )
     assert public_key1 == public_key2
 
     assert ca_cert.issuer == ca_cert.subject
     assert_is_ca(ca_cert)
 
     with pytest.raises(ValueError):
         ca.issue_cert()
 
-    server = ca.issue_cert(u"test-1.example.org", u"test-2.example.org")
+    server = ca.issue_cert(
+        "test-1.example.org", "test-2.example.org", key_type=key_type
+    )
 
     assert b"PRIVATE KEY" in server.private_key_pem.bytes()
     assert b"BEGIN CERTIFICATE" in server.cert_chain_pems[0].bytes()
     assert len(server.cert_chain_pems) == 1
     assert server.private_key_pem.bytes() in server.private_key_and_cert_chain_pem.bytes()
     for blob in server.cert_chain_pems:
         assert blob.bytes() in server.private_key_and_cert_chain_pem.bytes()
 
-    server_cert = x509.load_pem_x509_certificate(
-        server.cert_chain_pems[0].bytes(), default_backend())
+    server_cert = x509.load_pem_x509_certificate(server.cert_chain_pems[0].bytes())
 
     assert server_cert.not_valid_before <= today <= server_cert.not_valid_after
     assert server_cert.issuer == ca_cert.subject
     assert_is_leaf(server_cert)
 
     san = server_cert.extensions.get_extension_for_class(x509.SubjectAlternativeName)
     hostnames = san.value.get_values_for_type(x509.DNSName)
-    assert hostnames == [u"test-1.example.org", u"test-2.example.org"]
+    assert hostnames == ["test-1.example.org", "test-2.example.org"]
 
 
-def test_ca_custom_names():
-    # type: () -> None
+def test_ca_custom_names() -> None:
     ca = CA(
-        organization_name=u'python-trio',
-        organization_unit_name=u'trustme',
+        organization_name='python-trio',
+        organization_unit_name='trustme',
     )
 
-    ca_cert = x509.load_pem_x509_certificate(
-        ca.cert_pem.bytes(),
-        default_backend(),
-    )
+    ca_cert = x509.load_pem_x509_certificate(ca.cert_pem.bytes())
 
     assert {
         'O=python-trio',
         'OU=trustme',
     }.issubset({
         rdn.rfc4514_string()
         for rdn in ca_cert.subject.rdns
     })
 
 
-def test_issue_cert_custom_names():
-    # type: () -> None
+def test_issue_cert_custom_names() -> None:
     ca = CA()
     leaf_cert = ca.issue_cert(
-        u'example.org',
-        organization_name=u'python-trio',
-        organization_unit_name=u'trustme',
+        'example.org',
+        organization_name='python-trio',
+        organization_unit_name='trustme',
     )
 
-    cert = x509.load_pem_x509_certificate(
-        leaf_cert.cert_chain_pems[0].bytes(),
-        default_backend(),
-    )
+    cert = x509.load_pem_x509_certificate(leaf_cert.cert_chain_pems[0].bytes())
 
     assert {
         'O=python-trio',
         'OU=trustme',
     }.issubset({
         rdn.rfc4514_string()
         for rdn in cert.subject.rdns
     })
 
 
-def test_issue_cert_custom_not_after():
-    # type: () -> None
-     now = datetime.datetime.now()
-     expires = datetime.datetime(2025, 12, 1, 8, 10, 10)
-     ca = CA()
-
-     leaf_cert = ca.issue_cert(
-         u'example.org',
-         organization_name=u'python-trio',
-         organization_unit_name=u'trustme',
-         not_after=expires,
-     )
-
-     cert = x509.load_pem_x509_certificate(
-         leaf_cert.cert_chain_pems[0].bytes(),
-         default_backend(),
-     )
+def test_issue_cert_custom_not_after() -> None:
+    now = datetime.datetime.now()
+    expires = datetime.datetime(2025, 12, 1, 8, 10, 10)
+    ca = CA()
+
+    leaf_cert = ca.issue_cert(
+        "example.org",
+        organization_name="python-trio",
+        organization_unit_name="trustme",
+        not_after=expires,
+    )
+
+    cert = x509.load_pem_x509_certificate(leaf_cert.cert_chain_pems[0].bytes())
 
-     for t in ["year", "month", "day", "hour", "minute", "second"]:
-         assert getattr(cert.not_valid_after, t) == getattr(expires, t)
+    for t in ["year", "month", "day", "hour", "minute", "second"]:
+        assert getattr(cert.not_valid_after, t) == getattr(expires, t)
 
 
-def test_intermediate():
-    # type: () -> None
+def test_intermediate() -> None:
     ca = CA()
-    ca_cert = x509.load_pem_x509_certificate(
-        ca.cert_pem.bytes(), default_backend())
+    ca_cert = x509.load_pem_x509_certificate(ca.cert_pem.bytes())
     assert_is_ca(ca_cert)
     assert ca_cert.issuer == ca_cert.subject
     assert _path_length(ca_cert) == 9
 
     child_ca = ca.create_child_ca()
-    child_ca_cert = x509.load_pem_x509_certificate(
-        child_ca.cert_pem.bytes(), default_backend())
+    child_ca_cert = x509.load_pem_x509_certificate(child_ca.cert_pem.bytes())
     assert_is_ca(child_ca_cert)
     assert child_ca_cert.issuer == ca_cert.subject
     assert _path_length(child_ca_cert) == 8
 
-    child_server = child_ca.issue_cert(u"test-host.example.org")
+    child_server = child_ca.issue_cert("test-host.example.org")
     assert len(child_server.cert_chain_pems) == 2
     child_server_cert = x509.load_pem_x509_certificate(
-        child_server.cert_chain_pems[0].bytes(), default_backend())
+        child_server.cert_chain_pems[0].bytes()
+    )
     assert child_server_cert.issuer == child_ca_cert.subject
     assert_is_leaf(child_server_cert)
 
 
-def test_path_length():
-    # type: () -> None
+def test_path_length() -> None:
     ca = CA()
-    ca_cert = x509.load_pem_x509_certificate(
-        ca.cert_pem.bytes(), default_backend())
+    ca_cert = x509.load_pem_x509_certificate(ca.cert_pem.bytes())
     assert _path_length(ca_cert) == 9
 
     child_ca = ca
     for i in range(9):
         child_ca = child_ca.create_child_ca()
 
     # Can't create new child CAs anymore
-    child_ca_cert = x509.load_pem_x509_certificate(
-        child_ca.cert_pem.bytes(), default_backend())
+    child_ca_cert = x509.load_pem_x509_certificate(child_ca.cert_pem.bytes())
     assert _path_length(child_ca_cert) == 0
     with pytest.raises(ValueError):
         child_ca.create_child_ca()
 
 
-def test_unrecognized_context_type():
-    # type: () -> None
+def test_unrecognized_context_type() -> None:
     ca = CA()
-    server = ca.issue_cert(u"test-1.example.org")
+    server = ca.issue_cert("test-1.example.org")
 
     with pytest.raises(TypeError):
         ca.configure_trust(None)  # type: ignore[arg-type]
 
     with pytest.raises(TypeError):
         server.configure_cert(None)  # type: ignore[arg-type]
 
 
-def test_blob(tmpdir):
-    # type: (py.path.local) -> None
+def test_blob(tmp_path: Path) -> None:
     test_data = b"xyzzy"
     b = trustme.Blob(test_data)
 
     # bytes
 
     assert b.bytes() == test_data
 
     # write_to_path
 
-    b.write_to_path(str(tmpdir / "test1"))
-    with (tmpdir / "test1").open("rb") as f:
+    b.write_to_path(str(tmp_path / "test1"))
+    with (tmp_path / "test1").open("rb") as f:
         assert f.read() == test_data
 
     # append=False overwrites
-    with (tmpdir / "test2").open("wb") as f:
+    with (tmp_path / "test2").open("wb") as f:
         f.write(b"asdf")
-    b.write_to_path(str(tmpdir / "test2"))
-    with (tmpdir / "test2").open("rb") as f:
+    b.write_to_path(str(tmp_path / "test2"))
+    with (tmp_path / "test2").open("rb") as f:
         assert f.read() == test_data
 
     # append=True appends
-    with (tmpdir / "test2").open("wb") as f:
+    with (tmp_path / "test2").open("wb") as f:
         f.write(b"asdf")
-    b.write_to_path(str(tmpdir / "test2"), append=True)
-    with (tmpdir / "test2").open("rb") as f:
+    b.write_to_path(str(tmp_path / "test2"), append=True)
+    with (tmp_path / "test2").open("rb") as f:
         assert f.read() == b"asdf" + test_data
 
     # tempfile
-    with b.tempfile(dir=str(tmpdir)) as path:
-        assert path.startswith(str(tmpdir))
+    with b.tempfile(dir=str(tmp_path)) as path:
+        assert path.startswith(str(tmp_path))
         assert path.endswith(".pem")
         with open(path, "rb") as f:
             assert f.read() == test_data
 
-def test_ca_from_pem(tmpdir):
-    # type: (py.path.local) -> None
+def test_ca_from_pem(tmp_path: Path) -> None:
     ca1 = trustme.CA()
     ca2 = trustme.CA.from_pem(ca1.cert_pem.bytes(), ca1.private_key_pem.bytes())
     assert ca1._certificate == ca2._certificate
     assert ca1.private_key_pem.bytes() == ca2.private_key_pem.bytes()
 
 
-def check_connection_end_to_end(wrap_client, wrap_server):
-    # type: (Callable[[CA, socket.socket, Text], SslSocket], Callable[[LeafCert, socket.socket], SslSocket]) -> None
+def check_connection_end_to_end(
+    wrap_client: Callable[[CA, socket.socket, str], SslSocket],
+    wrap_server: Callable[[LeafCert, socket.socket], SslSocket],
+    key_type: KeyType,
+) -> None:
     # Client side
-    def fake_ssl_client(ca, raw_client_sock, hostname):
-        # type: (CA, socket.socket, Text) -> None
+    def fake_ssl_client(ca: CA, raw_client_sock: socket.socket, hostname: str) -> None:
         try:
             wrapped_client_sock = wrap_client(ca, raw_client_sock, hostname)
             # Send and receive some data to prove the connection is good
             wrapped_client_sock.send(b"x")
             assert wrapped_client_sock.recv(1) == b"y"
             wrapped_client_sock.close()
         except:  # pragma: no cover
             sys.excepthook(*sys.exc_info())
             raise
         finally:
             raw_client_sock.close()
 
     # Server side
-    def fake_ssl_server(server_cert, raw_server_sock):
-        # type: (LeafCert, socket.socket) -> None
+    def fake_ssl_server(server_cert: LeafCert, raw_server_sock: socket.socket) -> None:
         try:
             wrapped_server_sock = wrap_server(server_cert, raw_server_sock)
             # Prove that we're connected
             assert wrapped_server_sock.recv(1) == b"x"
             wrapped_server_sock.send(b"y")
             wrapped_server_sock.close()
         except:  # pragma: no cover
             sys.excepthook(*sys.exc_info())
             raise
         finally:
             raw_server_sock.close()
 
-    def doit(ca, hostname, server_cert):
-        # type: (CA, Text, LeafCert) -> None
+    def doit(ca: CA, hostname: str, server_cert: LeafCert) -> None:
         # socketpair and ssl don't work together on py2, because... reasons.
         # So we need to do this the hard way.
         listener = socket.socket()
         listener.bind(("127.0.0.1", 0))
         listener.listen(1)
         raw_client_sock = socket.socket()
         raw_client_sock.connect(listener.getsockname())
@@ -332,197 +307,184 @@
         listener.close()
         with ThreadPoolExecutor(2) as tpe:
             f1 = tpe.submit(fake_ssl_client, ca, raw_client_sock, hostname)
             f2 = tpe.submit(fake_ssl_server, server_cert, raw_server_sock)
             f1.result()
             f2.result()
 
-    ca = CA()
-    intermediate_ca = ca.create_child_ca()
-    hostname = u"my-test-host.example.org"
+    ca = CA(key_type=key_type)
+    intermediate_ca = ca.create_child_ca(key_type=key_type)
+    hostname = "my-test-host.example.org"
 
     # Should work
-    doit(ca, hostname, ca.issue_cert(hostname))
+    doit(ca, hostname, ca.issue_cert(hostname, key_type=key_type))
 
     # Should work
-    doit(ca, hostname, intermediate_ca.issue_cert(hostname))
+    doit(ca, hostname, intermediate_ca.issue_cert(hostname, key_type=key_type))
 
     # To make sure that the above success actually required that the
     # CA and cert logic is all working, make sure that the same code
     # fails if the certs or CA aren't right:
 
     # Bad hostname fails
     with pytest.raises(Exception):
-        doit(ca, u"asdf.example.org", ca.issue_cert(hostname))
+        doit(ca, "asdf.example.org", ca.issue_cert(hostname, key_type=key_type))
 
     # Bad CA fails
     bad_ca = CA()
     with pytest.raises(Exception):
-        doit(bad_ca, hostname, ca.issue_cert(hostname))
+        doit(bad_ca, hostname, ca.issue_cert(hostname, key_type=key_type))
 
 
-def test_stdlib_end_to_end():
-    # type: () -> None
-    def wrap_client(ca, raw_client_sock, hostname):
-        # type: (CA, socket.socket, Text) -> ssl.SSLSocket
+@pytest.mark.parametrize("key_type", [KeyType.RSA, KeyType.ECDSA])
+def test_stdlib_end_to_end(key_type: KeyType) -> None:
+    def wrap_client(ca: CA, raw_client_sock: socket.socket, hostname: str) -> ssl.SSLSocket:
         ctx = ssl.create_default_context()
         ca.configure_trust(ctx)
-        # Type ignore for Python 2: wants str, got unicode, but I guess unicode also works.
         wrapped_client_sock = ctx.wrap_socket(
-            raw_client_sock, server_hostname=hostname)  # type: ignore[arg-type]
+            raw_client_sock, server_hostname=hostname)
         print("Client got server cert:", wrapped_client_sock.getpeercert())
         peercert = wrapped_client_sock.getpeercert()
         assert peercert is not None
         san = peercert["subjectAltName"]
         assert san == (("DNS", "my-test-host.example.org"),)
         return wrapped_client_sock
 
-    def wrap_server(server_cert, raw_server_sock):
-        # type: (LeafCert, socket.socket) -> ssl.SSLSocket
+    def wrap_server(server_cert: LeafCert, raw_server_sock: socket.socket) -> ssl.SSLSocket:
         ctx = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
         server_cert.configure_cert(ctx)
         wrapped_server_sock = ctx.wrap_socket(
             raw_server_sock, server_side=True)
         print("server encrypted with:", wrapped_server_sock.cipher())
         return wrapped_server_sock
 
-    check_connection_end_to_end(wrap_client, wrap_server)
+    check_connection_end_to_end(wrap_client, wrap_server, key_type)
 
 
-def test_pyopenssl_end_to_end():
-    # type: () -> None
-    def wrap_client(ca, raw_client_sock, hostname):
-        # type: (CA, socket.socket, Text) -> OpenSSL.SSL.Connection
+@pytest.mark.parametrize("key_type", [KeyType.RSA, KeyType.ECDSA])
+def test_pyopenssl_end_to_end(key_type: KeyType) -> None:
+    def wrap_client(ca: CA, raw_client_sock: socket.socket, hostname: str) -> OpenSSL.SSL.Connection:
         # Cribbed from example at
         #   https://service-identity.readthedocs.io/en/stable/api.html#service_identity.pyopenssl.verify_hostname
         ctx = OpenSSL.SSL.Context(OpenSSL.SSL.SSLv23_METHOD)
         ctx.set_verify(OpenSSL.SSL.VERIFY_PEER,
                        lambda conn, cert, errno, depth, ok: bool(ok))
         ca.configure_trust(ctx)
         conn = OpenSSL.SSL.Connection(ctx, raw_client_sock)
         conn.set_connect_state()
         conn.do_handshake()
         service_identity.pyopenssl.verify_hostname(conn, hostname)
         return conn
 
-    def wrap_server(server_cert, raw_server_sock):
-        # type: (LeafCert, socket.socket) -> OpenSSL.SSL.Connection
+    def wrap_server(server_cert: LeafCert, raw_server_sock: socket.socket) -> OpenSSL.SSL.Connection:
         ctx = OpenSSL.SSL.Context(OpenSSL.SSL.SSLv23_METHOD)
         server_cert.configure_cert(ctx)
 
         conn = OpenSSL.SSL.Connection(ctx, raw_server_sock)
         conn.set_accept_state()
         conn.do_handshake()
         return conn
 
-    check_connection_end_to_end(wrap_client, wrap_server)
+    check_connection_end_to_end(wrap_client, wrap_server, key_type)
 
 
-def test_identity_variants():
-    # type: () -> None
+def test_identity_variants() -> None:
     ca = CA()
 
     for bad in [b"example.org", bytearray(b"example.org"), 123]:
         with pytest.raises(TypeError):
             ca.issue_cert(bad)  # type: ignore[arg-type]
 
     cases = {
         # Traditional ascii hostname
-        u"example.org": x509.DNSName(u"example.org"),
+        "example.org": x509.DNSName("example.org"),
 
         # Wildcard
-        u"*.example.org": x509.DNSName(u"*.example.org"),
+        "*.example.org": x509.DNSName("*.example.org"),
 
         # IDN
-        u"éxamplë.org": x509.DNSName(u"xn--xampl-9rat.org"),
-        u"xn--xampl-9rat.org": x509.DNSName(u"xn--xampl-9rat.org"),
+        "éxamplë.org": x509.DNSName("xn--xampl-9rat.org"),
+        "xn--xampl-9rat.org": x509.DNSName("xn--xampl-9rat.org"),
 
         # IDN + wildcard
-        u"*.éxamplë.org": x509.DNSName(u"*.xn--xampl-9rat.org"),
-        u"*.xn--xampl-9rat.org": x509.DNSName(u"*.xn--xampl-9rat.org"),
+        "*.éxamplë.org": x509.DNSName("*.xn--xampl-9rat.org"),
+        "*.xn--xampl-9rat.org": x509.DNSName("*.xn--xampl-9rat.org"),
 
         # IDN that acts differently in IDNA-2003 vs IDNA-2008
-        u"faß.de": x509.DNSName(u"xn--fa-hia.de"),
-        u"xn--fa-hia.de": x509.DNSName(u"xn--fa-hia.de"),
+        "faß.de": x509.DNSName("xn--fa-hia.de"),
+        "xn--fa-hia.de": x509.DNSName("xn--fa-hia.de"),
 
         # IDN with non-permissable character (uppercase K)
         # (example taken from idna package docs)
-        u"Königsgäßchen.de": x509.DNSName(u"xn--knigsgchen-b4a3dun.de"),
+        "Königsgäßchen.de": x509.DNSName("xn--knigsgchen-b4a3dun.de"),
 
         # IP addresses
-        u"127.0.0.1": x509.IPAddress(IPv4Address(u"127.0.0.1")),
-        u"::1": x509.IPAddress(IPv6Address(u"::1")),
+        "127.0.0.1": x509.IPAddress(IPv4Address("127.0.0.1")),
+        "::1": x509.IPAddress(IPv6Address("::1")),
         # Check normalization
-        u"0000::1": x509.IPAddress(IPv6Address(u"::1")),
+        "0000::1": x509.IPAddress(IPv6Address("::1")),
 
         # IP networks
-        u"127.0.0.0/24": x509.IPAddress(IPv4Network(u"127.0.0.0/24")),
-        u"2001::/16": x509.IPAddress(IPv6Network(u"2001::/16")),
+        "127.0.0.0/24": x509.IPAddress(IPv4Network("127.0.0.0/24")),
+        "2001::/16": x509.IPAddress(IPv6Network("2001::/16")),
         # Check normalization
-        u"2001:0000::/16": x509.IPAddress(IPv6Network(u"2001::/16")),
+        "2001:0000::/16": x509.IPAddress(IPv6Network("2001::/16")),
 
         # Email address
-        u"example@example.com": x509.RFC822Name(u"example@example.com"),
+        "example@example.com": x509.RFC822Name("example@example.com"),
     }
 
     for hostname, expected in cases.items():
         # Can't repr the got or expected values here, at least until
         # cryptography v2.1 is out, because in v2.0 on py2, DNSName.__repr__
         # blows up on IDNs.
-        print("testing: {!r}".format(hostname))
+        print(f"testing: {hostname!r}")
         pem = ca.issue_cert(hostname).cert_chain_pems[0].bytes()
-        cert = x509.load_pem_x509_certificate(pem, default_backend())
+        cert = x509.load_pem_x509_certificate(pem)
         san = cert.extensions.get_extension_for_class(
             x509.SubjectAlternativeName
         )
         assert_is_leaf(cert)
         got = list(san.value)[0]
         assert got == expected
 
 
-def test_backcompat():
-    # type: () -> None
+def test_backcompat() -> None:
     ca = CA()
     # We can still use the old name
-    ca.issue_server_cert(u"example.com")
+    ca.issue_server_cert("example.com")
 
 
-def test_CN():
-    # type: () -> None
+def test_CN() -> None:
     ca = CA()
 
-    # Since we have to emulate kwonly args here, I guess we should test the
-    # emulation logic
-    with pytest.raises(TypeError):
-        ca.issue_cert(comon_nam=u"wrong kwarg name")  # type: ignore[call-arg]
-
-    # Must be unicode
+    # Must be str
     with pytest.raises(TypeError):
         ca.issue_cert(common_name=b"bad kwarg value")  # type: ignore[arg-type]
 
     # Default is no common name
-    pem = ca.issue_cert(u"example.com").cert_chain_pems[0].bytes()
-    cert = x509.load_pem_x509_certificate(pem, default_backend())
+    pem = ca.issue_cert("example.com").cert_chain_pems[0].bytes()
+    cert = x509.load_pem_x509_certificate(pem)
     common_names = cert.subject.get_attributes_for_oid(
         x509.oid.NameOID.COMMON_NAME
     )
     assert common_names == []
 
     # Common name on its own is valid
-    pem = ca.issue_cert(common_name=u"woo").cert_chain_pems[0].bytes()
-    cert = x509.load_pem_x509_certificate(pem, default_backend())
+    pem = ca.issue_cert(common_name="woo").cert_chain_pems[0].bytes()
+    cert = x509.load_pem_x509_certificate(pem)
     common_names = cert.subject.get_attributes_for_oid(
         x509.oid.NameOID.COMMON_NAME
     )
-    assert common_names[0].value == u"woo"
+    assert common_names[0].value == "woo"
 
     # Common name + SAN
-    pem = ca.issue_cert(u"example.com", common_name=u"woo").cert_chain_pems[0].bytes()
-    cert = x509.load_pem_x509_certificate(pem, default_backend())
+    pem = ca.issue_cert("example.com", common_name="woo").cert_chain_pems[0].bytes()
+    cert = x509.load_pem_x509_certificate(pem)
     san = cert.extensions.get_extension_for_class(
         x509.SubjectAlternativeName
     )
-    assert list(san.value)[0] == x509.DNSName(u"example.com")
+    assert list(san.value)[0] == x509.DNSName("example.com")
     common_names = cert.subject.get_attributes_for_oid(
         x509.oid.NameOID.COMMON_NAME
     )
-    assert common_names[0].value == u"woo"
+    assert common_names[0].value == "woo"
```

### Comparing `trustme-0.9.0/trustme/__init__.py` & `trustme-1.0.0/src/trustme/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,89 +1,77 @@
-# -*- coding: utf-8 -*-
-
+from __future__ import annotations
 import datetime
+import ipaddress
+import os
 import ssl
+from enum import Enum
 from base64 import urlsafe_b64encode
-from tempfile import NamedTemporaryFile
 from contextlib import contextmanager
-import os
+from tempfile import NamedTemporaryFile
+from typing import Generator, List, Optional, Union, TYPE_CHECKING
 
-import ipaddress
-import idna  # type: ignore[import]
+import idna
 
 from cryptography import x509
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes
-from cryptography.hazmat.primitives.asymmetric import rsa
+from cryptography.hazmat.primitives.asymmetric import rsa, ec
 from cryptography.hazmat.primitives.serialization import (
     PrivateFormat, NoEncryption
 )
 from cryptography.x509.oid import ExtendedKeyUsageOID, NameOID
 from cryptography.hazmat.primitives.serialization import Encoding
 from cryptography.hazmat.primitives.serialization import load_pem_private_key
 
 from ._version import __version__
 
-TYPE_CHECKING = False
 if TYPE_CHECKING:  # pragma: no cover
-    from typing import Generator, List, Optional, Text, Union
-
     import OpenSSL.SSL
+    CERTIFICATE_PUBLIC_KEY_TYPES = Union[rsa.RSAPublicKey, ec.EllipticCurvePublicKey]
+    CERTIFICATE_PRIVATE_KEY_TYPES = Union[rsa.RSAPrivateKey, ec.EllipticCurvePrivateKey]
 
 __all__ = ["CA"]
 
-# Python 2/3 annoyingness
-try:
-    unicode
-except NameError:
-    unicode = str
-
-# On my laptop, making a CA + server certificate using 2048 bit keys takes ~160
-# ms, and using 4096 bit keys takes ~2 seconds. We want tests to run in 160 ms,
-# not 2 seconds. And we can't go lower, since Debian (and probably others)
-# by default reject any keys with <2048 bits (see #45).
-_KEY_SIZE = 2048
-
 # Default certificate expiry date:
 # OpenSSL on Windows fails if you try to give it a date after
 # ~3001-01-19:
 #   https://github.com/pyca/cryptography/issues/3194
 # Some versions of cryptography on 32-bit platforms fail if you give
 # them dates after ~2038-01-19:
 #   https://github.com/pyca/cryptography/pull/4658
 DEFAULT_EXPIRY = datetime.datetime(2038, 1, 1)
 
-def _name(name, organization_name=None, common_name=None):
-    # type: (Text, Optional[Text], Optional[Text]) -> x509.Name
+def _name(name: str, organization_name: Optional[str] = None, common_name: Optional[str] = None) -> x509.Name:
     name_pieces = [
         x509.NameAttribute(
             NameOID.ORGANIZATION_NAME,
-            organization_name or u"trustme v{}".format(__version__),
+            organization_name or f"trustme v{__version__}",
         ),
         x509.NameAttribute(NameOID.ORGANIZATIONAL_UNIT_NAME, name),
     ]
     if common_name is not None:
         name_pieces.append(
             x509.NameAttribute(NameOID.COMMON_NAME, common_name)
         )
     return x509.Name(name_pieces)
 
 
-def random_text():
-    # type: () -> Text
+def random_text() -> str:
     return urlsafe_b64encode(os.urandom(12)).decode("ascii")
 
 
-def _smells_like_pyopenssl(ctx):
-    # type: (object) -> bool
+def _smells_like_pyopenssl(ctx: object) -> bool:
     return getattr(ctx, "__module__", "").startswith("OpenSSL")  # type: ignore[no-any-return]
 
 
-def _cert_builder_common(subject, issuer, public_key, not_after=None):
-    # type: (x509.Name, x509.Name, rsa.RSAPublicKey, Optional[datetime.datetime]) -> x509.CertificateBuilder
+def _cert_builder_common(
+    subject: x509.Name,
+    issuer: x509.Name,
+    public_key: CERTIFICATE_PUBLIC_KEY_TYPES,
+    not_after: Optional[datetime.datetime] = None,
+) -> x509.CertificateBuilder:
     not_after = not_after if not_after else DEFAULT_EXPIRY
     return (
         x509.CertificateBuilder()
         .subject_name(subject)
         .issuer_name(issuer)
         .public_key(public_key)
         .not_valid_before(datetime.datetime(2000, 1, 1))
@@ -92,16 +80,15 @@
         .add_extension(
             x509.SubjectKeyIdentifier.from_public_key(public_key),
             critical=False,
         )
     )
 
 
-def _identity_string_to_x509(identity):
-    # type: (Text) -> x509.GeneralName
+def _identity_string_to_x509(identity: str) -> x509.GeneralName:
     # Because we are a DWIM library for lazy slackers, we cheerfully pervert
     # the cryptography library's carefully type-safe API, and silently DTRT
     # for any of the following identity types:
     #
     # - "example.org"
     # - "example.org"
     # - "éxamplë.org"
@@ -110,18 +97,18 @@
     # - "127.0.0.1"
     # - "::1"
     # - "10.0.0.0/8"
     # - "2001::/16"
     # - "example@example.org"
     #
     # plus wildcard variants of the identities.
-    if not isinstance(identity, unicode):
-        raise TypeError("identities must be text (unicode on py2, str on py3)")
+    if not isinstance(identity, str):
+        raise TypeError("identities must be str")
 
-    if u"@" in identity:
+    if "@" in identity:
         return x509.RFC822Name(identity)
 
     # Have to try ip_address first, because ip_network("127.0.0.1") is
     # interpreted as being the network 127.0.0.1/32. Which I guess would be
     # fine, actually, but why risk it.
     try:
         return x509.IPAddress(ipaddress.ip_address(identity))
@@ -138,35 +125,32 @@
         alabel_bytes = idna.encode(identity, uts46=True)
     # Then back to text, which is mandatory on cryptography 2.0 and earlier,
     # and may or may not be deprecated in cryptography 2.1.
     alabel = alabel_bytes.decode("ascii")
     return x509.DNSName(alabel)
 
 
-class Blob(object):
+class Blob:
     """A convenience wrapper for a blob of bytes.
 
     This type has no public constructor. They're used to provide a handy
     interface to the PEM-encoded data generated by `trustme`. For example, see
     `CA.cert_pem` or `LeafCert.private_key_and_cert_chain_pem`.
 
     """
-    def __init__(self, data):
-        # type: (bytes) -> None
+    def __init__(self, data: bytes) -> None:
         self._data = data
 
-    def bytes(self):
-        # type: () -> bytes
+    def bytes(self) -> bytes:
         """Returns the data as a `bytes` object.
 
         """
         return self._data
 
-    def write_to_path(self, path, append=False):
-        # type: (str, bool) -> None
+    def write_to_path(self, path: str, append: bool = False) -> None:
         """Writes the data to the file at the given path.
 
         Args:
           path (str): The path to write to.
           append (bool): If False (the default), replace any existing file
                with the given name. If True, append to any existing file.
 
@@ -175,25 +159,24 @@
             mode = "ab"
         else:
             mode = "wb"
         with open(path, mode) as f:
             f.write(self._data)
 
     @contextmanager
-    def tempfile(self, dir=None):
-        # type: (Optional[str]) -> Generator[str, None, None]
+    def tempfile(self, dir: Optional[str] = None) -> Generator[str, None, None]:
         """Context manager for writing data to a temporary file.
 
         The file is created when you enter the context manager, and
         automatically deleted when the context manager exits.
 
         Many libraries have annoying APIs which require that certificates be
         specified as filesystem paths, so even if you have already the data in
         memory, you have to write it out to disk and then let them read it
-        back in again. If you encouter such a library, you should probably
+        back in again. If you encounter such a library, you should probably
         file a bug. But in the mean time, this context manager makes it easy
         to give them what they want.
 
         Example:
 
           Here's how to get requests to use a trustme CA (`see also
           <http://docs.python-requests.org/en/master/user/advanced/#ssl-cert-verification>`__)::
@@ -206,49 +189,62 @@
           dir (str or None): Passed to `tempfile.NamedTemporaryFile`.
 
         """
         # On Windows, you can't re-open a NamedTemporaryFile that's still
         # open. Which seems like it completely defeats the purpose of having a
         # NamedTemporaryFile? Oh well...
         # https://bugs.python.org/issue14243
-        # Type ignore temporarily needed for Python 2:
-        # https://github.com/python/typeshed/pull/5836
-        f = NamedTemporaryFile(suffix=".pem", dir=dir, delete=False)  # type: ignore[arg-type]
+        f = NamedTemporaryFile(suffix=".pem", dir=dir, delete=False)
         try:
             f.write(self._data)
             f.close()
             yield f.name
         finally:
             f.close()  # in case write() raised an error
             os.unlink(f.name)
 
 
-class CA(object):
-    """A certificate authority."""
+class KeyType(Enum):
+    """Type of the key used to generate a certificate"""
 
-    _certificate = None  # type: x509.Certificate
+    RSA = 0
+    ECDSA = 1
+
+    def _generate_key(self) -> CERTIFICATE_PRIVATE_KEY_TYPES:
+        if self is KeyType.RSA:
+            # key_size needs to be a least 2048 to be accepted
+            # on Debian and pressumably other OSes
+
+            return rsa.generate_private_key(
+                public_exponent=65537, key_size=2048
+            )
+        elif self is KeyType.ECDSA:
+            return ec.generate_private_key(ec.SECP256R1())
+        else:  # pragma: no cover
+            raise ValueError("Unknown key type")
+
+
+class CA:
+    """A certificate authority."""
+    _certificate: x509.Certificate
 
     def __init__(
         self,
-        parent_cert=None,
-        path_length=9,
-        organization_name=None,
-        organization_unit_name=None,
-    ):
-        # type: (Optional[CA], int, Optional[Text], Optional[Text]) -> None
+        parent_cert: Optional["CA"] = None,
+        path_length: int = 9,
+        organization_name: Optional[str] = None,
+        organization_unit_name: Optional[str] = None,
+        key_type: KeyType = KeyType.ECDSA,
+    ) -> None:
         self.parent_cert = parent_cert
-        self._private_key = rsa.generate_private_key(
-            public_exponent=65537,
-            key_size=_KEY_SIZE,
-            backend=default_backend()
-        )
+        self._private_key = key_type._generate_key()
         self._path_length = path_length
 
         name = _name(
-            organization_unit_name or u"Testing CA #" + random_text(),
+            organization_unit_name or "Testing CA #" + random_text(),
             organization_name=organization_name,
         )
         issuer = name
         sign_key = self._private_key
         if parent_cert is not None:
             sign_key = parent_cert._private_key
             parent_certificate = parent_cert._certificate
@@ -272,66 +268,62 @@
                     encipher_only=False,
                     decipher_only=False),
                 critical=True
             )
             .sign(
                 private_key=sign_key,
                 algorithm=hashes.SHA256(),
-                backend=default_backend(),
             )
         )
 
     @property
-    def cert_pem(self):
-        # type: () -> Blob
+    def cert_pem(self) -> Blob:
         """`Blob`: The PEM-encoded certificate for this CA. Add this to your
         trust store to trust this CA."""
         return Blob(self._certificate.public_bytes(Encoding.PEM))
 
     @property
-    def private_key_pem(self):
-        # type: () -> Blob
+    def private_key_pem(self) -> Blob:
         """`Blob`: The PEM-encoded private key for this CA. Use this to sign
         other certificates from this CA."""
         return Blob(
             self._private_key.private_bytes(
                 Encoding.PEM,
                 PrivateFormat.TraditionalOpenSSL,
                 NoEncryption()
                 )
             )
 
-    def create_child_ca(self):
-        # type: () -> CA
+    def create_child_ca(self, key_type: KeyType = KeyType.ECDSA) -> "CA":
         """Creates a child certificate authority
 
         Returns:
           CA: the newly-generated certificate authority
 
         Raises:
           ValueError: if the CA path length is 0
         """
         if self._path_length == 0:
             raise ValueError("Can't create child CA: path length is 0")
 
         path_length = self._path_length - 1
-        return CA(parent_cert=self, path_length=path_length)
-
-    def issue_cert(self, *identities, **kwargs):
-        # type: (Text, Optional[Union[Text, datetime.datetime]]) -> LeafCert
-        # PY3: (str, Optional[str], Optional[str], Optional[str], Optional[datetime.datetime]) -> LeafCert
-        """issue_cert(*identities, common_name=None, organization_name=None, \
-        organization_unit_name=None, not_after=None)
+        return CA(parent_cert=self, path_length=path_length, key_type=key_type)
 
-        Issues a certificate. The certificate can be used for either servers
+    def issue_cert(
+        self,
+        *identities: str,
+        common_name: Optional[str] = None,
+        organization_name: Optional[str] = None,
+        organization_unit_name: Optional[str] = None,
+        not_after: Optional[datetime.datetime] = None,
+        key_type: KeyType = KeyType.ECDSA,
+    ) -> "LeafCert":
+        """Issues a certificate. The certificate can be used for either servers
         or clients.
 
-        All arguments must be text strings (``unicode`` on Python 2, ``str``
-        on Python 3).
-
         Args:
           identities: The identities that this certificate will be valid for.
             Most commonly, these are just hostnames, but we accept any of the
             following forms:
 
             - Regular hostname: ``example.com``
             - Wildcard hostname: ``*.example.com``
@@ -361,52 +353,35 @@
           organization_unit_name: Sets the "Organization Unit Name" (OU)
             attribute on the certificate. By default, a random one will be
             generated.
 
           not_after: Set the expiry date (notAfter) of the certificate. This
             argument type is `datetime.datetime`.
 
+          key_type: Set the type of key that is used for the certificate. By default this is an ECDSA based key.
+
         Returns:
           LeafCert: the newly-generated certificate.
 
         """
-        common_name = kwargs.pop("common_name", None)  # type: Optional[Text]  # type: ignore[assignment]
-        organization_name = kwargs.pop("organization_name", None)  # type: Optional[Text]  # type: ignore[assignment]
-        organization_unit_name = kwargs.pop("organization_unit_name", None)  # type: Optional[Text]  # type: ignore[assignment]
-        not_after = kwargs.pop("not_after", None)  # type: Optional[datetime.datetime]  # type: ignore[assignment]
-        if kwargs:
-            raise TypeError("unrecognized keyword arguments {}".format(kwargs))
-
         if not identities and common_name is None:
             raise ValueError(
                 "Must specify at least one identity or common name"
             )
 
-        key = rsa.generate_private_key(
-            public_exponent=65537,
-            key_size=_KEY_SIZE,
-            backend=default_backend()
-        )
+        key = key_type._generate_key()
 
         ski_ext = self._certificate.extensions.get_extension_for_class(
             x509.SubjectKeyIdentifier)
-        ski = ski_ext.value
-        # Workaround a bug in cryptography 2.6 and earlier, where you have to
-        # pass the extension object instead of the actual SKI object
-        try:
-            # The new way
-            aki = x509.AuthorityKeyIdentifier.from_issuer_subject_key_identifier(ski)
-        except AttributeError:
-            # The old way
-            aki = x509.AuthorityKeyIdentifier.from_issuer_subject_key_identifier(ski_ext)  # type: ignore[arg-type]
+        aki = x509.AuthorityKeyIdentifier.from_issuer_subject_key_identifier(ski_ext.value)
 
         cert = (
             _cert_builder_common(
                 _name(
-                    organization_unit_name or u"Testing cert #" + random_text(),
+                    organization_unit_name or "Testing cert #" + random_text(),
                     organization_name=organization_name,
                     common_name=common_name,
                 ),
                 self._certificate.subject,
                 key.public_key(),
                 not_after=not_after,
             )
@@ -441,15 +416,14 @@
                     ExtendedKeyUsageOID.CODE_SIGNING,
                 ]),
                 critical=True
             )
             .sign(
                 private_key=self._private_key,
                 algorithm=hashes.SHA256(),
-                backend=default_backend(),
             )
         )
 
         chain_to_ca = []
         ca = self
         while ca.parent_cert is not None:
             chain_to_ca.append(ca._certificate.public_bytes(Encoding.PEM))
@@ -464,16 +438,15 @@
                 cert.public_bytes(Encoding.PEM),
                 chain_to_ca,
             )
 
     # For backwards compatibility
     issue_server_cert = issue_cert
 
-    def configure_trust(self, ctx):
-        # type: (Union[ssl.SSLContext, OpenSSL.SSL.Context]) -> None
+    def configure_trust(self, ctx: Union[ssl.SSLContext, "OpenSSL.SSL.Context"]) -> None:
         """Configure the given context object to trust certificates signed by
         this CA.
 
         Args:
           ctx (ssl.SSLContext or OpenSSL.SSL.Context): The SSL context to be
               modified.
 
@@ -489,35 +462,33 @@
             store.add_cert(cert)
         else:
             raise TypeError(
                 "unrecognized context type {!r}"
                 .format(ctx.__class__.__name__))
 
     @classmethod
-    def from_pem(cls, cert_bytes, private_key_bytes):
-        # type: (bytes, bytes) -> CA
+    def from_pem(cls, cert_bytes: bytes, private_key_bytes: bytes) -> "CA":
         """Build a CA from existing cert and private key.
 
         This is useful if your test suite has an existing certificate authority and
         you're not ready to switch completely to trustme just yet.
 
         Args:
           cert_bytes (bytes): The bytes of the certificate in PEM format
           private_key_bytes (bytes): The bytes of the private key in PEM format
         """
         ca = cls()
         ca.parent_cert = None
-        ca._certificate = x509.load_pem_x509_certificate(
-            cert_bytes, backend=default_backend())
-        ca._private_key = load_pem_private_key(
-            private_key_bytes, password=None, backend=default_backend())
+        ca._certificate = x509.load_pem_x509_certificate(cert_bytes)
+        ca._private_key = load_pem_private_key(private_key_bytes, password=None)  # type: ignore[assignment]
+
         return ca
 
 
-class LeafCert(object):
+class LeafCert:
     """A server or client certificate.
 
     This type has no public constructor; you get one by calling
     `CA.issue_cert` or similar.
 
     Attributes:
       private_key_pem (`Blob`): The PEM-encoded private key corresponding to
@@ -528,24 +499,22 @@
           are the rest of the certificate chain needed to reach the root CA.
 
       private_key_and_cert_chain_pem (`Blob`): A single `Blob` containing the
           concatenation of the PEM-encoded private key and the PEM-encoded
           cert chain.
 
     """
-    def __init__(self, private_key_pem, server_cert_pem, chain_to_ca):
-        # type: (bytes, bytes, List[bytes]) -> None
+    def __init__(self, private_key_pem: bytes, server_cert_pem: bytes, chain_to_ca: List[bytes]) -> None:
         self.private_key_pem = Blob(private_key_pem)
         self.cert_chain_pems = [
             Blob(pem) for pem in [server_cert_pem] + chain_to_ca]
         self.private_key_and_cert_chain_pem = (
             Blob(private_key_pem + server_cert_pem + b''.join(chain_to_ca)))
 
-    def configure_cert(self, ctx):
-        # type: (Union[ssl.SSLContext, OpenSSL.SSL.Context]) -> None
+    def configure_cert(self, ctx: Union[ssl.SSLContext, "OpenSSL.SSL.Context"]) -> None:
         """Configure the given context object to present this certificate.
 
         Args:
           ctx (ssl.SSLContext or OpenSSL.SSL.Context): The SSL context to be
               modified.
 
         """
```

### Comparing `trustme-0.9.0/trustme/_cli.py` & `trustme-1.0.0/src/trustme/_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,19 @@
-# -*- coding: utf-8 -*-
-
 import argparse
 import os
 import trustme
 import sys
-
+from typing import List, Optional
 from datetime import datetime
 
-TYPE_CHECKING = False
-if TYPE_CHECKING:  # pragma: no cover
-    from typing import List, Optional
-
-# Python 2/3 annoyingness
-try:
-    unicode
-except NameError:  # pragma: no cover
-    unicode = str
 
 # ISO 8601
 DATE_FORMAT = '%Y-%m-%d'
 
-def main(argv=None):
-    # type: (Optional[List[str]]) -> None
+def main(argv: Optional[List[str]] = None) -> None:
     if argv is None:
         argv = sys.argv[1:]
 
     parser = argparse.ArgumentParser(prog="trustme")
     parser.add_argument(
         "-d",
         "--dir",
@@ -54,30 +42,37 @@
     )
     parser.add_argument(
         "-q",
         "--quiet",
         action="store_true",
         help="Doesn't print out helpful information for humans.",
     )
+    parser.add_argument(
+        "-k",
+        "--key-type",
+        choices=list(t.name for t in trustme.KeyType),
+        default="ECDSA",
+    )
 
     args = parser.parse_args(argv)
     cert_dir = args.dir
-    identities = [unicode(identity) for identity in args.identities]
-    common_name = unicode(args.common_name[0]) if args.common_name else None
+    identities = [str(identity) for identity in args.identities]
+    common_name = str(args.common_name[0]) if args.common_name else None
     expires_on = None if args.expires_on is None else datetime.strptime(args.expires_on, DATE_FORMAT)
     quiet = args.quiet
+    key_type = trustme.KeyType[args.key_type]
 
     if not os.path.isdir(cert_dir):
-        raise ValueError("--dir={} is not a directory".format(cert_dir))
+        raise ValueError(f"--dir={cert_dir} is not a directory")
     if len(identities) < 1:
         raise ValueError("Must include at least one identity")
 
     # Generate the CA certificate
-    ca = trustme.CA()
-    cert = ca.issue_cert(*identities, common_name=common_name, not_after=expires_on)
+    ca = trustme.CA(key_type=key_type)
+    cert = ca.issue_cert(*identities, common_name=common_name, not_after=expires_on, key_type=key_type)
 
     # Write the certificate and private key the server should use
     server_key = os.path.join(cert_dir, "server.key")
     server_cert = os.path.join(cert_dir, "server.pem")
     cert.private_key_pem.write_to_path(path=server_key)
     with open(server_cert, mode="w") as f:
         f.truncate()
@@ -86,13 +81,13 @@
 
     # Write the certificate the client should trust
     client_cert = os.path.join(cert_dir, "client.pem")
     ca.cert_pem.write_to_path(path=client_cert)
 
     if not quiet:
         idents = "', '".join(identities)
-        print("Generated a certificate for '{}'".format(idents))
+        print(f"Generated a certificate for '{idents}'")
         print("Configure your server to use the following files:")
-        print("  cert={}".format(server_cert))
-        print("  key={}".format(server_key))
+        print(f"  cert={server_cert}")
+        print(f"  key={server_key}")
         print("Configure your client to use the following files:")
-        print("  cert={}".format(client_cert))
+        print(f"  cert={client_cert}")
```

### Comparing `trustme-0.9.0/trustme.egg-info/PKG-INFO` & `trustme-1.0.0/src/trustme.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,160 +1,162 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: trustme
-Version: 0.9.0
+Version: 1.0.0
 Summary: #1 quality TLS certs while you wait, for the discerning tester
 Home-page: https://github.com/python-trio/trustme
 Author: Nathaniel J. Smith
 Author-email: njs@pobox.com
-License: MIT -or- Apache License 2.0
-Description: .. note that this README gets 'include'ed into the main documentation
-        
-        ==============================================
-         trustme: #1 quality TLS certs while you wait
-        ==============================================
-        
-        .. image:: https://vignette2.wikia.nocookie.net/jadensadventures/images/1/1e/Kaa%27s_hypnotic_eyes.jpg/revision/latest?cb=20140310173415
-           :width: 200px
-           :align: right
-        
-        You wrote a cool network client or server. It encrypts connections
-        using `TLS
-        <https://en.wikipedia.org/wiki/Transport_Layer_Security>`__. Your test
-        suite needs to make TLS connections to itself.
-        
-        Uh oh. Your test suite *probably* doesn't have a valid TLS
-        certificate. Now what?
-        
-        ``trustme`` is a tiny Python package that does one thing: it gives you
-        a `fake <https://martinfowler.com/bliki/TestDouble.html>`__
-        certificate authority (CA) that you can use to generate fake TLS certs
-        to use in your tests. Well, technically they're real certs, they're
-        just signed by your CA, which nobody trusts. But you can trust
-        it. Trust me.
-        
-        
-        Vital statistics
-        ================
-        
-        **Install:** ``pip install -U trustme``
-        
-        **Documentation:** https://trustme.readthedocs.io
-        
-        **Bug tracker and source code:** https://github.com/python-trio/trustme
-        
-        **Tested on:** Python 2.7 and Python 3.5+, CPython and PyPy
-        
-        **License:** MIT or Apache 2, your choice.
-        
-        **Code of conduct:** Contributors are requested to follow our `code of
-        conduct
-        <https://github.com/python-trio/trustme/blob/master/CODE_OF_CONDUCT.md>`__
-        in all project spaces.
-        
-        
-        Cheat sheet
-        ===========
-        
-        Programmatic usage:
-        
-        .. code-block:: python
-        
-           import trustme
-        
-           # ----- Creating certs -----
-        
-           # Look, you just created your certificate authority!
-           ca = trustme.CA()
-        
-           # And now you issued a cert signed by this fake CA
-           # https://en.wikipedia.org/wiki/Example.org
-           server_cert = ca.issue_cert(u"test-host.example.org")
-        
-           # That's it!
-        
-           # ----- Using your shiny new certs -----
-        
-           # You can configure SSL context objects to trust this CA:
-           ca.configure_trust(ssl_context)
-           # Or configure them to present the server certificate
-           server_cert.configure_cert(ssl_context)
-           # You can use standard library or PyOpenSSL context objects here,
-           # trustme is happy either way.
-        
-           # ----- or -----
-                        
-           # Save the PEM-encoded data to a file to use in non-Python test
-           # suites:
-           ca.cert_pem.write_to_path("ca.pem")
-           server_cert.private_key_and_cert_chain_pem.write_to_path("server.pem")
-           
-           # ----- or -----
-                        
-           # Put the PEM-encoded data in a temporary file, for libraries that
-           # insist on that:
-           with ca.cert_pem.tempfile() as ca_temp_path:
-               requests.get("https://...", verify=ca_temp_path)
-        
-        Command line usage:
-        
-        .. code-block:: console
-        
-           $ # Certs may be generated from anywhere. Here's where we are:
-           $ pwd
-           /tmp
-           $ # ----- Creating certs -----
-           $ python -m trustme
-           Generated a certificate for 'localhost', '127.0.0.1', '::1'
-           Configure your server to use the following files:
-             cert=/tmp/server.pem
-             key=/tmp/server.key
-           Configure your client to use the following files:
-             cert=/tmp/client.pem
-           $ # ----- Using certs -----
-           $ gunicorn --keyfile server.key --certfile server.pem app:app
-           $ curl --cacert client.pem https://localhost:8000/
-           Hello, world!
-        
-        
-        FAQ
-        ===
-        
-        **Should I use these certs for anything real?** Certainly not.
-        
-        **Why not just use self-signed certificates?** These are more
-        realistic. You don't have to disable your certificate validation code
-        in your test suite, which is good because you want to test what you
-        run in production, and you would *never* disable your certificate
-        validation code in production, right? Plus, they're just as easy to
-        work with. Actually easier, in many cases.
-        
-        **What if I want to test how my code handles some bizarre TLS
-        configuration?** We think trustme hits a sweet spot of ease-of-use
-        and generality as it is. The defaults are carefully chosen to work
-        on all major operating systems and be as fast as possible. We don't
-        want to turn trustme into a second-rate re-export of everything in
-        `cryptography <https://cryptography.io>`__. If you have more complex
-        needs, consider using them directly, possibly starting from the
-        trustme code.
-        
-        **Will you automate installing CA cert into system trust store?** No.
-        `mkcert <https://github.com/FiloSottile/mkcert>`__ already does this
-        well, and we would not have anything to add.
-        
-Platform: UNKNOWN
+License: MIT OR Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Networking
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
+License-File: LICENSE
+License-File: LICENSE.APACHE2
+License-File: LICENSE.MIT
+
+.. note that this README gets 'include'ed into the main documentation
+
+==============================================
+ trustme: #1 quality TLS certs while you wait
+==============================================
+
+.. image:: https://vignette2.wikia.nocookie.net/jadensadventures/images/1/1e/Kaa%27s_hypnotic_eyes.jpg/revision/latest?cb=20140310173415
+   :width: 200px
+   :align: right
+
+You wrote a cool network client or server. It encrypts connections
+using `TLS
+<https://en.wikipedia.org/wiki/Transport_Layer_Security>`__. Your test
+suite needs to make TLS connections to itself.
+
+Uh oh. Your test suite *probably* doesn't have a valid TLS
+certificate. Now what?
+
+``trustme`` is a tiny Python package that does one thing: it gives you
+a `fake <https://martinfowler.com/bliki/TestDouble.html>`__
+certificate authority (CA) that you can use to generate fake TLS certs
+to use in your tests. Well, technically they're real certs, they're
+just signed by your CA, which nobody trusts. But you can trust
+it. Trust me.
+
+
+Vital statistics
+================
+
+**Install:** ``pip install -U trustme``
+
+**Documentation:** https://trustme.readthedocs.io
+
+**Bug tracker and source code:** https://github.com/python-trio/trustme
+
+**Tested on:** Python 3.7+, CPython and PyPy
+
+**License:** MIT or Apache 2, your choice.
+
+**Code of conduct:** Contributors are requested to follow our `code of
+conduct
+<https://github.com/python-trio/trustme/blob/master/CODE_OF_CONDUCT.md>`__
+in all project spaces.
+
+
+Cheat sheet
+===========
+
+Programmatic usage:
+
+.. code-block:: python
+
+   import trustme
+
+   # ----- Creating certs -----
+
+   # Look, you just created your certificate authority!
+   ca = trustme.CA()
+
+   # And now you issued a cert signed by this fake CA
+   # https://en.wikipedia.org/wiki/Example.org
+   server_cert = ca.issue_cert(u"test-host.example.org")
+
+   # That's it!
+
+   # ----- Using your shiny new certs -----
+
+   # You can configure SSL context objects to trust this CA:
+   ca.configure_trust(ssl_context)
+   # Or configure them to present the server certificate
+   server_cert.configure_cert(ssl_context)
+   # You can use standard library or PyOpenSSL context objects here,
+   # trustme is happy either way.
+
+   # ----- or -----
+                
+   # Save the PEM-encoded data to a file to use in non-Python test
+   # suites:
+   ca.cert_pem.write_to_path("ca.pem")
+   server_cert.private_key_and_cert_chain_pem.write_to_path("server.pem")
+   
+   # ----- or -----
+                
+   # Put the PEM-encoded data in a temporary file, for libraries that
+   # insist on that:
+   with ca.cert_pem.tempfile() as ca_temp_path:
+       requests.get("https://...", verify=ca_temp_path)
+
+Command line usage:
+
+.. code-block:: console
+
+   $ # Certs may be generated from anywhere. Here's where we are:
+   $ pwd
+   /tmp
+   $ # ----- Creating certs -----
+   $ python -m trustme
+   Generated a certificate for 'localhost', '127.0.0.1', '::1'
+   Configure your server to use the following files:
+     cert=/tmp/server.pem
+     key=/tmp/server.key
+   Configure your client to use the following files:
+     cert=/tmp/client.pem
+   $ # ----- Using certs -----
+   $ gunicorn --keyfile server.key --certfile server.pem app:app
+   $ curl --cacert client.pem https://localhost:8000/
+   Hello, world!
+
+
+FAQ
+===
+
+**Should I use these certs for anything real?** Certainly not.
+
+**Why not just use self-signed certificates?** These are more
+realistic. You don't have to disable your certificate validation code
+in your test suite, which is good because you want to test what you
+run in production, and you would *never* disable your certificate
+validation code in production, right? Plus, they're just as easy to
+work with. Actually easier, in many cases.
+
+**What if I want to test how my code handles some bizarre TLS
+configuration?** We think trustme hits a sweet spot of ease-of-use
+and generality as it is. The defaults are carefully chosen to work
+on all major operating systems and be as fast as possible. We don't
+want to turn trustme into a second-rate re-export of everything in
+`cryptography <https://cryptography.io>`__. If you have more complex
+needs, consider using them directly, possibly starting from the
+trustme code.
+
+**Will you automate installing CA cert into system trust store?** No.
+`mkcert <https://github.com/FiloSottile/mkcert>`__ already does this
+well, and we would not have anything to add.
```

### Comparing `trustme-0.9.0/trustme.egg-info/SOURCES.txt` & `trustme-1.0.0/src/trustme.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 CODE_OF_CONDUCT.md
 LICENSE
 LICENSE.APACHE2
 LICENSE.MIT
 MANIFEST.in
 README.rst
 pyproject.toml
-setup.cfg
 setup.py
 test-requirements.txt
 docs/Makefile
 docs/make.bat
 docs/source/conf.py
 docs/source/index.rst
 docs/source/trustme-trio-example.py
 docs/source/_static/.gitkeep
 docs/source/_templates/need-help.html
+src/trustme/__init__.py
+src/trustme/__main__.py
+src/trustme/_cli.py
+src/trustme/_version.py
+src/trustme/py.typed
+src/trustme.egg-info/PKG-INFO
+src/trustme.egg-info/SOURCES.txt
+src/trustme.egg-info/dependency_links.txt
+src/trustme.egg-info/requires.txt
+src/trustme.egg-info/top_level.txt
 tests/test_cli.py
-tests/test_trustme.py
-trustme/__init__.py
-trustme/__main__.py
-trustme/_cli.py
-trustme/_version.py
-trustme/py.typed
-trustme.egg-info/PKG-INFO
-trustme.egg-info/SOURCES.txt
-trustme.egg-info/dependency_links.txt
-trustme.egg-info/requires.txt
-trustme.egg-info/top_level.txt
+tests/test_trustme.py
```

