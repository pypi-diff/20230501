# Comparing `tmp/requests-toolbelt-0.9.1.tar.gz` & `tmp/requests-toolbelt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/requests-toolbelt-0.9.1.tar", last modified: Wed Jan 30 01:29:41 2019, max compression
+gzip compressed data, was "requests-toolbelt-1.0.0.tar", last modified: Mon May  1 04:09:40 2023, max compression
```

## Comparing `requests-toolbelt-0.9.1.tar` & `requests-toolbelt-1.0.0.tar`

### file list

```diff
@@ -1,121 +1,118 @@
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     9568 2019-01-30 01:28:28.000000 requests-toolbelt-0.9.1/HISTORY.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      595 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/LICENSE
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3337 2017-06-03 00:35:47.000000 requests-toolbelt-0.9.1/README.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1032 2019-01-30 01:28:21.000000 requests-toolbelt-0.9.1/tox.ini
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/tests/
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/tests/cassettes/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     5993 2018-10-08 11:43:24.000000 requests-toolbelt-0.9.1/tests/cassettes/file_for_download.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1158 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/cassettes/httpbin_guess_auth_none.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)   159879 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/cassettes/stream_response_to_file.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      935 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/cassettes/klevas_vu_lt_ssl3.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1866 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/cassettes/http2bin_cookies.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2077 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/cassettes/httpbin_guess_auth_digest.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1008 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/cassettes/simple_get_request.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      958 2019-01-29 17:43:40.000000 requests-toolbelt-0.9.1/tests/cassettes/test_x509_adapter_pem.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1565 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/cassettes/httpbin_guess_auth_basic.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1121 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/cassettes/http2bin_fingerprint.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      958 2019-01-29 17:43:40.000000 requests-toolbelt-0.9.1/tests/cassettes/test_x509_adapter_der.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4887 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/cassettes/redirect_request_for_dump_all.json
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2087 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_multipart_monitor.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)    13458 2019-01-29 17:43:33.000000 requests-toolbelt-0.9.1/tests/test_dump.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4033 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_proxy_digest_auth.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2182 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_auth_handler.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)    10868 2018-10-08 11:43:24.000000 requests-toolbelt-0.9.1/tests/test_multipart_encoder.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     7350 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_downloadutils.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3865 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_socket_options_adapter.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3759 2017-05-20 21:20:06.000000 requests-toolbelt-0.9.1/tests/test_user_agent.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2068 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_formdata.py
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/tests/certs/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1941 2019-01-29 17:43:40.000000 requests-toolbelt-0.9.1/tests/certs/test_cert.p12
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2689 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_auth.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1019 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_ssladapter.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      709 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_fingerprintadapter.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      769 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_forgetfulcookiejar.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1160 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_source_adapter.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2044 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_streaming_iterator.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      160 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/__init__.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      321 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/conftest.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1572 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_host_header_ssl_adapter.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3065 2019-01-29 17:43:40.000000 requests-toolbelt-0.9.1/tests/test_x509_adapter.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     6895 2018-01-05 12:36:25.000000 requests-toolbelt-0.9.1/tests/test_multipart_decoder.py
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/tests/threaded/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     7934 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/threaded/test_pool.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4746 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/threaded/test_thread.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1948 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/threaded/test_api.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)        0 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/threaded/__init__.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3509 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_appengine_adapter.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      951 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/tests/test_sessions.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2038 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/setup.py
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt/
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt/utils/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2558 2017-03-25 11:07:58.000000 requests-toolbelt-0.9.1/requests_toolbelt/utils/deprecated.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3233 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/utils/formdata.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4524 2017-05-20 21:20:06.000000 requests-toolbelt-0.9.1/requests_toolbelt/utils/user_agent.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)        0 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/utils/__init__.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     6490 2019-01-29 17:43:33.000000 requests-toolbelt-0.9.1/requests_toolbelt/utils/dump.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4044 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/streaming_iterator.py
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt/adapters/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2399 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/adapters/ssl.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     7324 2019-01-29 17:43:40.000000 requests-toolbelt-0.9.1/requests_toolbelt/adapters/x509.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2608 2018-01-05 12:36:25.000000 requests-toolbelt-0.9.1/requests_toolbelt/adapters/source.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      363 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/adapters/__init__.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1404 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/adapters/fingerprint.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     7540 2017-03-25 11:07:58.000000 requests-toolbelt-0.9.1/requests_toolbelt/adapters/appengine.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1396 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/adapters/host_header_ssl.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4789 2017-06-03 00:35:47.000000 requests-toolbelt-0.9.1/requests_toolbelt/adapters/socket_options.py
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt/downloadutils/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     6069 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/downloadutils/stream.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4365 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/downloadutils/tee.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)        0 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/downloadutils/__init__.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     9893 2019-01-30 01:26:45.000000 requests-toolbelt-0.9.1/requests_toolbelt/_compat.py
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt/multipart/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)    20772 2018-10-08 11:43:24.000000 requests-toolbelt-0.9.1/requests_toolbelt/multipart/encoder.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4861 2018-10-08 11:43:24.000000 requests-toolbelt-0.9.1/requests_toolbelt/multipart/decoder.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      847 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/multipart/__init__.py
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt/cookies/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      213 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/cookies/forgetful.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)        0 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/cookies/__init__.py
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt/auth/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3705 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/auth/http_proxy_digest.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      910 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/auth/_digest_auth_compat.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4408 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/auth/handler.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)        0 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/auth/__init__.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4944 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/auth/guess.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1135 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/exceptions.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2321 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/sessions.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1181 2019-01-30 01:27:51.000000 requests-toolbelt-0.9.1/requests_toolbelt/__init__.py
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt/threaded/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1465 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/requests_toolbelt/threaded/thread.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     6628 2018-01-05 12:36:25.000000 requests-toolbelt-0.9.1/requests_toolbelt/threaded/pool.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3213 2017-06-03 00:35:47.000000 requests-toolbelt-0.9.1/requests_toolbelt/threaded/__init__.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     2501 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/CODE_OF_CONDUCT.rst
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt.egg-info/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)        1 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt.egg-info/dependency_links.txt
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3193 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt.egg-info/SOURCES.txt
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)       23 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt.egg-info/requires.txt
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)    17441 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt.egg-info/PKG-INFO
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)       18 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/requests_toolbelt.egg-info/top_level.txt
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)    17441 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/PKG-INFO
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      902 2019-01-29 17:43:40.000000 requests-toolbelt-0.9.1/AUTHORS.rst
-drwxrwxr-x   0 icordasc  (1000) icordasc  (1000)        0 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/docs/
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      659 2019-01-29 17:43:33.000000 requests-toolbelt-0.9.1/docs/dumputils.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     8841 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/conf.py
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4843 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/threading.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      634 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/sessions.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4665 2017-06-03 00:35:47.000000 requests-toolbelt-0.9.1/docs/contributing.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     9344 2019-01-29 17:43:40.000000 requests-toolbelt-0.9.1/docs/adapters.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      408 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/downloadutils.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)       38 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/user.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      180 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/formdata.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     3166 2017-05-20 21:20:06.000000 requests-toolbelt-0.9.1/docs/user-agent.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     6806 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/Makefile
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      239 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/exceptions.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     1056 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/index.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     6360 2019-01-29 17:43:40.000000 requests-toolbelt-0.9.1/docs/uploading-data.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     4678 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/authentication.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      386 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/deprecated.rst
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)     6723 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/docs/make.bat
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)       64 2019-01-29 17:43:40.000000 requests-toolbelt-0.9.1/dev-requirements.txt
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)      305 2017-01-19 14:23:03.000000 requests-toolbelt-0.9.1/MANIFEST.in
--rw-rw-r--   0 icordasc  (1000) icordasc  (1000)       61 2019-01-30 01:29:41.000000 requests-toolbelt-0.9.1/setup.cfg
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.044419 requests-toolbelt-1.0.0/
+-rw-r--r--   0 q         (1000) q         (1000)      986 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/AUTHORS.rst
+-rw-r--r--   0 q         (1000) q         (1000)     2511 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 q         (1000) q         (1000)    10170 2023-04-29 20:16:00.000000 requests-toolbelt-1.0.0/HISTORY.rst
+-rw-r--r--   0 q         (1000) q         (1000)      596 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/LICENSE
+-rw-r--r--   0 q         (1000) q         (1000)      305 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/MANIFEST.in
+-rw-r--r--   0 q         (1000) q         (1000)    14597 2023-05-01 04:09:40.044419 requests-toolbelt-1.0.0/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)     2978 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/README.rst
+-rw-r--r--   0 q         (1000) q         (1000)       93 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/dev-requirements.txt
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.036419 requests-toolbelt-1.0.0/docs/
+-rw-r--r--   0 q         (1000) q         (1000)     6806 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/docs/Makefile
+-rw-r--r--   0 q         (1000) q         (1000)     7366 2023-04-29 20:07:08.000000 requests-toolbelt-1.0.0/docs/adapters.rst
+-rw-r--r--   0 q         (1000) q         (1000)     4666 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/docs/authentication.rst
+-rw-r--r--   0 q         (1000) q         (1000)     8842 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/docs/conf.py
+-rw-r--r--   0 q         (1000) q         (1000)     4653 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/docs/contributing.rst
+-rw-r--r--   0 q         (1000) q         (1000)      384 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/docs/deprecated.rst
+-rw-r--r--   0 q         (1000) q         (1000)      408 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/docs/downloadutils.rst
+-rw-r--r--   0 q         (1000) q         (1000)      659 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/docs/dumputils.rst
+-rw-r--r--   0 q         (1000) q         (1000)      239 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/docs/exceptions.rst
+-rw-r--r--   0 q         (1000) q         (1000)      180 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/docs/formdata.rst
+-rw-r--r--   0 q         (1000) q         (1000)     1055 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/docs/index.rst
+-rw-r--r--   0 q         (1000) q         (1000)     6723 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/docs/make.bat
+-rw-r--r--   0 q         (1000) q         (1000)      634 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/docs/sessions.rst
+-rw-r--r--   0 q         (1000) q         (1000)     4833 2023-04-28 11:44:13.000000 requests-toolbelt-1.0.0/docs/threading.rst
+-rw-r--r--   0 q         (1000) q         (1000)     6360 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/docs/uploading-data.rst
+-rw-r--r--   0 q         (1000) q         (1000)     3166 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/docs/user-agent.rst
+-rw-r--r--   0 q         (1000) q         (1000)       38 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/docs/user.rst
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.037419 requests-toolbelt-1.0.0/requests_toolbelt/
+-rw-r--r--   0 q         (1000) q         (1000)     1188 2023-05-01 04:00:19.000000 requests-toolbelt-1.0.0/requests_toolbelt/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     9260 2023-04-29 20:07:08.000000 requests-toolbelt-1.0.0/requests_toolbelt/_compat.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.038419 requests-toolbelt-1.0.0/requests_toolbelt/adapters/
+-rw-r--r--   0 q         (1000) q         (1000)      370 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/requests_toolbelt/adapters/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     1404 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/adapters/fingerprint.py
+-rw-r--r--   0 q         (1000) q         (1000)     1396 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/adapters/host_header_ssl.py
+-rw-r--r--   0 q         (1000) q         (1000)     4789 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/requests_toolbelt/adapters/socket_options.py
+-rw-r--r--   0 q         (1000) q         (1000)     2608 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/adapters/source.py
+-rw-r--r--   0 q         (1000) q         (1000)     2399 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/adapters/ssl.py
+-rw-r--r--   0 q         (1000) q         (1000)     7854 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/requests_toolbelt/adapters/x509.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.038419 requests-toolbelt-1.0.0/requests_toolbelt/auth/
+-rw-r--r--   0 q         (1000) q         (1000)        0 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/auth/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)      910 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/auth/_digest_auth_compat.py
+-rw-r--r--   0 q         (1000) q         (1000)     4944 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/auth/guess.py
+-rw-r--r--   0 q         (1000) q         (1000)     4407 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/requests_toolbelt/auth/handler.py
+-rw-r--r--   0 q         (1000) q         (1000)     3706 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/requests_toolbelt/auth/http_proxy_digest.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.039420 requests-toolbelt-1.0.0/requests_toolbelt/cookies/
+-rw-r--r--   0 q         (1000) q         (1000)        0 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/cookies/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)      213 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/cookies/forgetful.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.039420 requests-toolbelt-1.0.0/requests_toolbelt/downloadutils/
+-rw-r--r--   0 q         (1000) q         (1000)        0 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/downloadutils/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     6024 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/requests_toolbelt/downloadutils/stream.py
+-rw-r--r--   0 q         (1000) q         (1000)     4365 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/downloadutils/tee.py
+-rw-r--r--   0 q         (1000) q         (1000)      695 2023-04-29 20:07:08.000000 requests-toolbelt-1.0.0/requests_toolbelt/exceptions.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.039420 requests-toolbelt-1.0.0/requests_toolbelt/multipart/
+-rw-r--r--   0 q         (1000) q         (1000)      854 2022-10-06 09:56:36.000000 requests-toolbelt-1.0.0/requests_toolbelt/multipart/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     4861 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/requests_toolbelt/multipart/decoder.py
+-rw-r--r--   0 q         (1000) q         (1000)    20769 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/requests_toolbelt/multipart/encoder.py
+-rw-r--r--   0 q         (1000) q         (1000)     3102 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/requests_toolbelt/sessions.py
+-rw-r--r--   0 q         (1000) q         (1000)     4044 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/streaming_iterator.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.040419 requests-toolbelt-1.0.0/requests_toolbelt/threaded/
+-rw-r--r--   0 q         (1000) q         (1000)     3213 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/threaded/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     6628 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/threaded/pool.py
+-rw-r--r--   0 q         (1000) q         (1000)     1465 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/threaded/thread.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.040419 requests-toolbelt-1.0.0/requests_toolbelt/utils/
+-rw-r--r--   0 q         (1000) q         (1000)        0 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/utils/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     2558 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/utils/deprecated.py
+-rw-r--r--   0 q         (1000) q         (1000)     6522 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/requests_toolbelt/utils/dump.py
+-rw-r--r--   0 q         (1000) q         (1000)     3233 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/utils/formdata.py
+-rw-r--r--   0 q         (1000) q         (1000)     4524 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/requests_toolbelt/utils/user_agent.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.037419 requests-toolbelt-1.0.0/requests_toolbelt.egg-info/
+-rw-r--r--   0 q         (1000) q         (1000)    14597 2023-05-01 04:09:39.000000 requests-toolbelt-1.0.0/requests_toolbelt.egg-info/PKG-INFO
+-rw-r--r--   0 q         (1000) q         (1000)     3163 2023-05-01 04:09:40.000000 requests-toolbelt-1.0.0/requests_toolbelt.egg-info/SOURCES.txt
+-rw-r--r--   0 q         (1000) q         (1000)        1 2023-05-01 04:09:39.000000 requests-toolbelt-1.0.0/requests_toolbelt.egg-info/dependency_links.txt
+-rw-r--r--   0 q         (1000) q         (1000)       23 2023-05-01 04:09:39.000000 requests-toolbelt-1.0.0/requests_toolbelt.egg-info/requires.txt
+-rw-r--r--   0 q         (1000) q         (1000)       18 2023-05-01 04:09:39.000000 requests-toolbelt-1.0.0/requests_toolbelt.egg-info/top_level.txt
+-rw-r--r--   0 q         (1000) q         (1000)       67 2023-05-01 04:09:40.045420 requests-toolbelt-1.0.0/setup.cfg
+-rw-r--r--   0 q         (1000) q         (1000)     2635 2023-04-28 11:44:13.000000 requests-toolbelt-1.0.0/setup.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.042420 requests-toolbelt-1.0.0/tests/
+-rw-r--r--   0 q         (1000) q         (1000)      160 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/__init__.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.044419 requests-toolbelt-1.0.0/tests/cassettes/
+-rw-r--r--   0 q         (1000) q         (1000)     5993 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/file_for_download.json
+-rw-r--r--   0 q         (1000) q         (1000)     1866 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/http2bin_cookies.json
+-rw-r--r--   0 q         (1000) q         (1000)     1121 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/http2bin_fingerprint.json
+-rw-r--r--   0 q         (1000) q         (1000)     1565 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/httpbin_guess_auth_basic.json
+-rw-r--r--   0 q         (1000) q         (1000)     2077 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/httpbin_guess_auth_digest.json
+-rw-r--r--   0 q         (1000) q         (1000)     1158 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/httpbin_guess_auth_none.json
+-rw-r--r--   0 q         (1000) q         (1000)      935 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/klevas_vu_lt_ssl3.json
+-rw-r--r--   0 q         (1000) q         (1000)     4887 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/redirect_request_for_dump_all.json
+-rw-r--r--   0 q         (1000) q         (1000)     1008 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/simple_get_request.json
+-rw-r--r--   0 q         (1000) q         (1000)   159879 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/stream_response_to_file.json
+-rw-r--r--   0 q         (1000) q         (1000)     3637 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/stream_response_without_content_length_to_file.json
+-rw-r--r--   0 q         (1000) q         (1000)      958 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/test_x509_adapter_der.json
+-rw-r--r--   0 q         (1000) q         (1000)      958 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tests/cassettes/test_x509_adapter_pem.json
+-rw-r--r--   0 q         (1000) q         (1000)      321 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/conftest.py
+-rw-r--r--   0 q         (1000) q         (1000)     2748 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_auth.py
+-rw-r--r--   0 q         (1000) q         (1000)     2182 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/test_auth_handler.py
+-rw-r--r--   0 q         (1000) q         (1000)     7409 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_downloadutils.py
+-rw-r--r--   0 q         (1000) q         (1000)    13517 2023-04-29 20:06:49.000000 requests-toolbelt-1.0.0/tests/test_dump.py
+-rw-r--r--   0 q         (1000) q         (1000)      709 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/test_fingerprintadapter.py
+-rw-r--r--   0 q         (1000) q         (1000)      769 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/test_forgetfulcookiejar.py
+-rw-r--r--   0 q         (1000) q         (1000)     2068 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/test_formdata.py
+-rw-r--r--   0 q         (1000) q         (1000)     1572 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/test_host_header_ssl_adapter.py
+-rw-r--r--   0 q         (1000) q         (1000)     6952 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_multipart_decoder.py
+-rw-r--r--   0 q         (1000) q         (1000)    10982 2023-04-28 11:44:13.000000 requests-toolbelt-1.0.0/tests/test_multipart_encoder.py
+-rw-r--r--   0 q         (1000) q         (1000)     2087 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/test_multipart_monitor.py
+-rw-r--r--   0 q         (1000) q         (1000)     4092 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_proxy_digest_auth.py
+-rw-r--r--   0 q         (1000) q         (1000)     2214 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_sessions.py
+-rw-r--r--   0 q         (1000) q         (1000)     4285 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_socket_options_adapter.py
+-rw-r--r--   0 q         (1000) q         (1000)     1225 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_source_adapter.py
+-rw-r--r--   0 q         (1000) q         (1000)     1078 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_ssladapter.py
+-rw-r--r--   0 q         (1000) q         (1000)     2044 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/test_streaming_iterator.py
+-rw-r--r--   0 q         (1000) q         (1000)     3824 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_user_agent.py
+-rw-r--r--   0 q         (1000) q         (1000)     3248 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/test_x509_adapter.py
+drwxr-xr-x   0 q         (1000) q         (1000)        0 2023-05-01 04:09:40.044419 requests-toolbelt-1.0.0/tests/threaded/
+-rw-r--r--   0 q         (1000) q         (1000)        0 2022-09-26 10:22:04.000000 requests-toolbelt-1.0.0/tests/threaded/__init__.py
+-rw-r--r--   0 q         (1000) q         (1000)     2007 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/threaded/test_api.py
+-rw-r--r--   0 q         (1000) q         (1000)     8185 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/threaded/test_pool.py
+-rw-r--r--   0 q         (1000) q         (1000)     4904 2022-10-31 12:14:08.000000 requests-toolbelt-1.0.0/tests/threaded/test_thread.py
+-rw-r--r--   0 q         (1000) q         (1000)     1498 2023-04-29 20:06:58.000000 requests-toolbelt-1.0.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `requests-toolbelt-0.9.1/HISTORY.rst` & `requests-toolbelt-1.0.0/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,84 @@
 History
 =======
 
+1.0.0 -- 2023-05-01
+-------------------
+
+Breaking Changes
+~~~~~~~~~~~~~~~~
+
+- Removed Google App Engine support to allow using urllib3 2.0
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Ensured the test suite no longer reaches the Internet
+
+Miscellaneous
+~~~~~~~~~~~~~
+
+- Added explicit support for Python 3.11
+
+0.10.1 -- 2022-10-25
+--------------------
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fix urllib3 warning to only emit on X509Adapter usage
+
+0.10.0 -- 2022-10-06
+--------------------
+
+New Features
+~~~~~~~~~~~~
+
+- Add support for preparing requests in BaseUrlSession
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fixing missing newline in dump utility
+
 0.9.1 -- 2019-01-29
 -------------------
 
 Fixed Bugs
 ~~~~~~~~~~
 
 - Fix import of pyOpenSSL shim from urllib3 for PKCS12 adapter
 
 0.9.0 -- 2019-01-29
 -------------------
 
 New Features
 ~~~~~~~~~~~~
 
-- Add X509 Adapter that can handle PKCS12 
+- Add X509 Adapter that can handle PKCS12
 - Add stateless solution for streaming files by MultipartEncoder from one host to another (in chunks)
 
 Fixed Bugs
 ~~~~~~~~~~
 
 - Update link to example
 - Move import of ``ABCs`` from collections into version-specific part of
   _compat module
 - Fix backwards incompatibility in ``get_encodings_from_content``
 - Correct callback documentation for ``MultipartEncoderMonitor``
 - Fix bug when ``MultipartEncoder`` is asked to encode zero parts
 - Correct the type of non string request body dumps
 - Removed content from being stored in MultipartDecoder
-- Fix bug by enabling support for contenttype with capital letters. 
+- Fix bug by enabling support for contenttype with capital letters.
 - Coerce proxy URL to bytes before dumping request
 - Avoid bailing out with exception upon empty response reason
 - Corrected Pool documentation
 - Corrected parentheses match in example usage
 - Fix "oject" to "object" in ``MultipartEncoder``
-- Fix URL for the project after the move 
+- Fix URL for the project after the move
 - Add fix for OSX TCPKeepAliveAdapter
 
 Miscellaneous
 ~~~~~~~~~~~~~
 
 - Remove py33 from testing and add Python 3.6 and nightly testing to the travis matrix.
 
@@ -229,15 +268,15 @@
 on the project's page.
 
 New Features
 ~~~~~~~~~~~~
 
 - A naive implemenation of a thread pool is now included in the toolbelt. See
   the docs in ``docs/threading.rst`` or on `Read The Docs
-  <https://toolbelt.readthedocs.org>`_.
+  <https://toolbelt.readthedocs.io/>`_.
 
 - The ``StreamingIterator`` now accepts files (such as ``sys.stdin``) without
   a specific length and will properly stream them.
 
 - The ``MultipartEncoder`` now accepts exactly the same format of fields as
   requests' ``files`` parameter does. In other words, you can now also pass in
   extra headers to add to a part in the body. You can also now specify a
```

### Comparing `requests-toolbelt-0.9.1/LICENSE` & `requests-toolbelt-1.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Copyright 2014 Ian Cordasco, Cory Benfield
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
-       http://www.apache.org/licenses/LICENSE-2.0
+       https://www.apache.org/licenses/LICENSE-2.0
 
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
```

### Comparing `requests-toolbelt-0.9.1/README.rst` & `requests-toolbelt-1.0.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 The Requests Toolbelt
 =====================
 
-This is just a collection of utilities for `python-requests`_, but don't 
-really belong in ``requests`` proper. The minimum tested requests version is 
-``2.1.0``. In reality, the toolbelt should work with ``2.0.1`` as well, but 
+This is just a collection of utilities for `python-requests`_, but don't
+really belong in ``requests`` proper. The minimum tested requests version is
+``2.1.0``. In reality, the toolbelt should work with ``2.0.1`` as well, but
 some idiosyncracies prevent effective or sane testing on that version.
 
 ``pip install requests-toolbelt`` to get started!
 
 
 multipart/form-data Encoder
 ---------------------------
@@ -64,54 +64,45 @@
 
     r = requests.get('https://api.github.com/users', headers=headers)
 
 
 SSLAdapter
 ----------
 
-The ``SSLAdapter`` was originally published on `Cory Benfield's blog`_. 
-This adapter allows the user to choose one of the SSL protocols made available 
+The ``SSLAdapter`` was originally published on `Cory Benfield's blog`_.
+This adapter allows the user to choose one of the SSL protocols made available
 in Python's ``ssl`` module for outgoing HTTPS connections:
 
 .. code-block:: python
 
     from requests_toolbelt import SSLAdapter
     import requests
     import ssl
 
     s = requests.Session()
     s.mount('https://', SSLAdapter(ssl.PROTOCOL_TLSv1))
 
 cookies/ForgetfulCookieJar
 --------------------------
 
-The ``ForgetfulCookieJar`` prevents a particular requests session from storing 
+The ``ForgetfulCookieJar`` prevents a particular requests session from storing
 cookies:
 
 .. code-block:: python
 
     from requests_toolbelt.cookies.forgetful import ForgetfulCookieJar
 
     session = requests.Session()
     session.cookies = ForgetfulCookieJar()
 
-Known Issues
-------------
-
-On Python 3.3.0 and 3.3.1, the standard library's ``http`` module will fail
-when passing an instance of the ``MultipartEncoder``. This is fixed in later
-minor releases of Python 3.3. Please consider upgrading to a later minor
-version or Python 3.4. *There is absolutely nothing this library can do to
-work around that bug.*
-
 Contributing
 ------------
 
 Please read the `suggested workflow
-<https://toolbelt.readthedocs.org/en/latest/contributing.html>`_ for
+<https://toolbelt.readthedocs.io/en/latest/contributing.html>`_ for
 contributing to this project.
 
 Please report any bugs on the `issue tracker`_
 
 .. _Cory Benfield's blog: https://lukasa.co.uk/2013/01/Choosing_SSL_Version_In_Requests/
 .. _python-requests: https://github.com/kennethreitz/requests
 .. _issue tracker: https://github.com/requests/toolbelt/issues
```

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/file_for_download.json` & `requests-toolbelt-1.0.0/tests/cassettes/file_for_download.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/httpbin_guess_auth_none.json` & `requests-toolbelt-1.0.0/tests/cassettes/httpbin_guess_auth_none.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/stream_response_to_file.json` & `requests-toolbelt-1.0.0/tests/cassettes/stream_response_to_file.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/klevas_vu_lt_ssl3.json` & `requests-toolbelt-1.0.0/tests/cassettes/klevas_vu_lt_ssl3.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/http2bin_cookies.json` & `requests-toolbelt-1.0.0/tests/cassettes/http2bin_cookies.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/httpbin_guess_auth_digest.json` & `requests-toolbelt-1.0.0/tests/cassettes/httpbin_guess_auth_digest.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/simple_get_request.json` & `requests-toolbelt-1.0.0/tests/cassettes/simple_get_request.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/test_x509_adapter_pem.json` & `requests-toolbelt-1.0.0/tests/cassettes/test_x509_adapter_der.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/httpbin_guess_auth_basic.json` & `requests-toolbelt-1.0.0/tests/cassettes/httpbin_guess_auth_basic.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/http2bin_fingerprint.json` & `requests-toolbelt-1.0.0/tests/cassettes/http2bin_fingerprint.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/test_x509_adapter_der.json` & `requests-toolbelt-1.0.0/tests/cassettes/test_x509_adapter_pem.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/cassettes/redirect_request_for_dump_all.json` & `requests-toolbelt-1.0.0/tests/cassettes/redirect_request_for_dump_all.json`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/test_multipart_monitor.py` & `requests-toolbelt-1.0.0/tests/test_multipart_monitor.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/test_dump.py` & `requests-toolbelt-1.0.0/tests/test_dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 This module, however, tests many of the private implementation details since
 those public functions just wrap them and testing the public functions will be
 very complex and high-level.
 """
 from requests_toolbelt._compat import HTTPHeaderDict
 from requests_toolbelt.utils import dump
 
-import mock
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 import pytest
 import requests
 
 from . import get_betamax
 
 HTTP_1_1 = 11
 HTTP_1_0 = 10
```

### Comparing `requests-toolbelt-0.9.1/tests/test_proxy_digest_auth.py` & `requests-toolbelt-1.0.0/tests/test_proxy_digest_auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # -*- coding: utf-8 -*-
 """Test proxy digest authentication."""
 
 import unittest
-import mock
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 
 import requests
 from requests_toolbelt.auth import http_proxy_digest
 
 
 class TestProxyDigestAuth(unittest.TestCase):
     """Tests for the ProxyDigestAuth class."""
```

### Comparing `requests-toolbelt-0.9.1/tests/test_auth_handler.py` & `requests-toolbelt-1.0.0/tests/test_auth_handler.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/test_multipart_encoder.py` & `requests-toolbelt-1.0.0/tests/test_multipart_encoder.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import unittest
 import io
 
 import requests
 
+import pytest
 from requests_toolbelt.multipart.encoder import (
     CustomBytesIO, MultipartEncoder, FileFromURLWrapper, FileNotSupportedError)
 from requests_toolbelt._compat import filepost
 from . import get_betamax
 
 
 preserve_bytes = {'preserve_exact_body_bytes': True}
@@ -87,22 +88,22 @@
         s = b'this is a unicode string: \xc3\xa9 \xc3\xa1 \xc7\xab \xc3\xb3'
         self.instance = CustomBytesIO(s)
         assert self.instance.read() == s
 
 
 class TestFileFromURLWrapper(unittest.TestCase):
     def setUp(self):
-        s = requests.Session()
-        self.recorder = get_betamax(s)
+        self.session = requests.Session()
+        self.recorder = get_betamax(self.session)
 
     def test_read_file(self):
         url = ('https://stxnext.com/static/img/logo.830ebe551641.svg')
         with self.recorder.use_cassette(
                 'file_for_download', **preserve_bytes):
-            self.instance = FileFromURLWrapper(url)
+            self.instance = FileFromURLWrapper(url, session=self.session)
             assert self.instance.len == 5177
             chunk = self.instance.read(20)
             assert chunk == b'<svg xmlns="http://w'
             assert self.instance.len == 5157
             chunk = self.instance.read(0)
             assert chunk == b''
             assert self.instance.len == 5157
@@ -112,17 +113,17 @@
 
     def test_no_content_length_header(self):
         url = (
             'https://api.github.com/repos/sigmavirus24/github3.py/releases/'
             'assets/37944'
         )
         with self.recorder.use_cassette(
-                'stream_response_to_file', **preserve_bytes):
+                'stream_response_without_content_length_to_file', **preserve_bytes):
             with self.assertRaises(FileNotSupportedError) as context:
-                FileFromURLWrapper(url)
+                FileFromURLWrapper(url, session=self.session)
             assert context.exception.__str__() == (
                 'Data from provided URL https://api.github.com/repos/s'
                 'igmavirus24/github3.py/releases/assets/37944 is not '
                 'supported. Lack of content-length Header in requested'
                 ' file response.'
             )
 
@@ -194,15 +195,15 @@
     def test_reads_file_from_url_wrapper(self):
         s = requests.Session()
         recorder = get_betamax(s)
         url = ('https://stxnext.com/static/img/logo.830ebe551641.svg')
         with recorder.use_cassette(
                 'file_for_download'):
             m = MultipartEncoder(
-                [('field', 'foo'), ('file', FileFromURLWrapper(url))])
+                [('field', 'foo'), ('file', FileFromURLWrapper(url, session=s))])
         assert m.read() is not None
 
     def test_reads_open_file_objects_with_a_specified_filename(self):
         with open('setup.py', 'rb') as fd:
             m = MultipartEncoder(
                 [('field', 'foo'), ('file', ('filename', fd, 'text/plain'))]
                 )
```

### Comparing `requests-toolbelt-0.9.1/tests/test_downloadutils.py` & `requests-toolbelt-1.0.0/tests/test_downloadutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 import os.path
 import shutil
 import tempfile
 
 import requests
 from requests_toolbelt.downloadutils import stream
 from requests_toolbelt.downloadutils import tee
-import mock
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 import pytest
 
 from . import get_betamax
 
 
 preserve_bytes = {'preserve_exact_body_bytes': True}
```

### Comparing `requests-toolbelt-0.9.1/tests/test_socket_options_adapter.py` & `requests-toolbelt-1.0.0/tests/test_socket_options_adapter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 # -*- coding: utf-8 -*-
 """Tests for the SocketOptionsAdapter and TCPKeepAliveAdapter."""
 import contextlib
+import platform
 import socket
+import sys
 
-import mock
+import pytest
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 import requests
 from requests_toolbelt._compat import poolmanager
 
 from requests_toolbelt.adapters import socket_options
 
 
 @contextlib.contextmanager
@@ -65,14 +71,16 @@
         pool_connections=10,
         pool_maxsize=5,
         pool_block=True,
     )
     assert PoolManager.called is False
 
 
+@pytest.mark.xfail(sys.version_info.major == 2 and platform.system() == "Windows",
+                   reason="Windows does not have TCP_KEEPINTVL in Python 2")
 @mock.patch.object(requests, '__build__', 0x020500)
 @mock.patch.object(poolmanager, 'PoolManager')
 def test_keep_alive_on_newer_requests_no_idle(PoolManager):
     """Show that options are generated correctly from kwargs."""
     socket_opts = [
         (socket.IPPROTO_TCP, socket.TCP_NODELAY, 1),
         (socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1),
@@ -89,14 +97,16 @@
     PoolManager.assert_called_once_with(
         num_pools=10, maxsize=5, block=True,
         socket_options=socket_opts
     )
     assert adapter.socket_options == socket_opts
 
 
+@pytest.mark.xfail(sys.version_info.major == 2 and platform.system() == "Windows",
+                   reason="Windows does not have TCP_KEEPINTVL in Python 2")
 @mock.patch.object(requests, '__build__', 0x020500)
 @mock.patch.object(poolmanager, 'PoolManager')
 def test_keep_alive_on_newer_requests_with_idle(PoolManager):
     """Show that options are generated correctly from kwargs with KEEPIDLE."""
     with set_keepidle(3000):
         socket_opts = [
             (socket.IPPROTO_TCP, socket.TCP_NODELAY, 1),
```

### Comparing `requests-toolbelt-0.9.1/tests/test_user_agent.py` & `requests-toolbelt-1.0.0/tests/test_user_agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # -*- coding: utf-8 -*-
 import unittest
 import sys
 
-from mock import patch
+try:
+    from unittest.mock import patch
+except ImportError:
+    from mock import patch
 import pytest
 
 from requests_toolbelt.utils import user_agent as ua
 
 
 class Object(object):
     """
```

### Comparing `requests-toolbelt-0.9.1/tests/test_formdata.py` & `requests-toolbelt-1.0.0/tests/test_formdata.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/test_auth.py` & `requests-toolbelt-1.0.0/tests/test_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # -*- coding: utf-8 -*-
 import requests
 import unittest
-import mock
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 
 from requests_toolbelt.auth.guess import GuessAuth, GuessProxyAuth
 from . import get_betamax
 
 
 class TestGuessAuth(unittest.TestCase):
     def setUp(self):
```

### Comparing `requests-toolbelt-0.9.1/tests/test_ssladapter.py` & `requests-toolbelt-1.0.0/tests/test_ssladapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # -*- coding: utf-8 -*-
-import mock
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 import pytest
 import requests
 import unittest
 
 from requests_toolbelt import SSLAdapter
 from . import get_betamax
```

### Comparing `requests-toolbelt-0.9.1/tests/test_fingerprintadapter.py` & `requests-toolbelt-1.0.0/tests/test_fingerprintadapter.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/test_forgetfulcookiejar.py` & `requests-toolbelt-1.0.0/tests/test_forgetfulcookiejar.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/test_source_adapter.py` & `requests-toolbelt-1.0.0/tests/test_source_adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # -*- coding: utf-8 -*-
 from requests.adapters import DEFAULT_POOLSIZE, DEFAULT_POOLBLOCK
-from mock import patch
+try:
+    from unittest.mock import patch
+except ImportError:
+    from mock import patch
 from requests_toolbelt.adapters.source import SourceAddressAdapter
 
 import pytest
 
 
 @patch('requests_toolbelt.adapters.source.poolmanager')
 def test_source_address_adapter_string(poolmanager):
```

### Comparing `requests-toolbelt-0.9.1/tests/test_streaming_iterator.py` & `requests-toolbelt-1.0.0/tests/test_streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/test_host_header_ssl_adapter.py` & `requests-toolbelt-1.0.0/tests/test_host_header_ssl_adapter.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/tests/test_x509_adapter.py` & `requests-toolbelt-1.0.0/tests/test_x509_adapter.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,83 @@
 # -*- coding: utf-8 -*-
 import requests
 import unittest
 import pytest
 
-from OpenSSL.crypto import load_pkcs12
-from cryptography.hazmat.primitives.serialization import (Encoding, 
-                                                          PrivateFormat,
-                                                          NoEncryption,
-                                                          BestAvailableEncryption)
+try:
+    import OpenSSL
+except ImportError:
+    PYOPENSSL_AVAILABLE = False
+else:
+    PYOPENSSL_AVAILABLE = True
+    from requests_toolbelt.adapters.x509 import X509Adapter
+    from cryptography import x509
+    from cryptography.hazmat.primitives.serialization import (
+        Encoding,
+        PrivateFormat,
+        BestAvailableEncryption,
+        load_pem_private_key,
+    )
+    import trustme
 
 from requests_toolbelt import exceptions as exc
-from requests_toolbelt.adapters.x509 import X509Adapter
 from . import get_betamax
 
 REQUESTS_SUPPORTS_SSL_CONTEXT = requests.__build__ >= 0x021200
 
+pytestmark = pytest.mark.filterwarnings(
+    "ignore:'urllib3.contrib.pyopenssl' module is deprecated:DeprecationWarning")
+
 
 class TestX509Adapter(unittest.TestCase):
     """Tests a simple requests.get() call using a .p12 cert.
     """
     def setUp(self):
-        with open('./tests/certs/test_cert.p12', 'rb') as pkcs12_file:
-            self.pkcs12_data = pkcs12_file.read()
-
         self.pkcs12_password_bytes = "test".encode('utf8')
         self.session = requests.Session()
 
     @pytest.mark.skipif(not REQUESTS_SUPPORTS_SSL_CONTEXT,
-                    reason="Requires Requests v2.12.0 or later")
+                        reason="Requires Requests v2.12.0 or later")
+    @pytest.mark.skipif(not PYOPENSSL_AVAILABLE,
+                        reason="Requires OpenSSL")
     def test_x509_pem(self):
-        p12 = load_pkcs12(self.pkcs12_data, self.pkcs12_password_bytes)
-        cert_bytes = p12.get_certificate().to_cryptography().public_bytes(Encoding.PEM)
-        pk_bytes = p12.get_privatekey().\
-                       to_cryptography_key().\
-                       private_bytes(Encoding.PEM, PrivateFormat.PKCS8, 
-                                     BestAvailableEncryption(self.pkcs12_password_bytes))
+        ca = trustme.CA()
+        cert = ca.issue_cert(u'pkiprojecttest01.dev.labs.internal')
+        cert_bytes = cert.cert_chain_pems[0].bytes()
+        pk_bytes = cert.private_key_pem.bytes()
 
-        adapter = X509Adapter(max_retries=3, cert_bytes=cert_bytes, 
-                              pk_bytes=pk_bytes, password=self.pkcs12_password_bytes)
+        adapter = X509Adapter(max_retries=3, cert_bytes=cert_bytes, pk_bytes=pk_bytes)
         self.session.mount('https://', adapter)
         recorder = get_betamax(self.session)
         with recorder.use_cassette('test_x509_adapter_pem'):
             r = self.session.get('https://pkiprojecttest01.dev.labs.internal/', verify=False)
 
         assert r.status_code == 200
         assert r.text
 
     @pytest.mark.skipif(not REQUESTS_SUPPORTS_SSL_CONTEXT,
                     reason="Requires Requests v2.12.0 or later")
-    def test_x509_der(self):
-        p12 = load_pkcs12(self.pkcs12_data, self.pkcs12_password_bytes)
-        cert_bytes = p12.get_certificate().to_cryptography().public_bytes(Encoding.DER)
-        pk_bytes = p12.get_privatekey().to_cryptography_key().private_bytes(Encoding.DER, PrivateFormat.PKCS8, NoEncryption())
-        adapter = X509Adapter(max_retries=3, cert_bytes=cert_bytes, pk_bytes=pk_bytes, encoding=Encoding.DER)
+    @pytest.mark.skipif(not PYOPENSSL_AVAILABLE,
+                    reason="Requires OpenSSL")
+    def test_x509_der_and_password(self):
+        ca = trustme.CA()
+        cert = ca.issue_cert(u'pkiprojecttest01.dev.labs.internal')
+        cert_bytes = x509.load_pem_x509_certificate(
+            cert.cert_chain_pems[0].bytes()).public_bytes(Encoding.DER)
+        pem_pk = load_pem_private_key(cert.private_key_pem.bytes(), password=None)
+        pk_bytes = pem_pk.private_bytes(Encoding.DER, PrivateFormat.PKCS8,
+                                        BestAvailableEncryption(self.pkcs12_password_bytes))
+
+        adapter = X509Adapter(max_retries=3, cert_bytes=cert_bytes, pk_bytes=pk_bytes,
+                              password=self.pkcs12_password_bytes, encoding=Encoding.DER)
         self.session.mount('https://', adapter)
         recorder = get_betamax(self.session)
         with recorder.use_cassette('test_x509_adapter_der'):
             r = self.session.get('https://pkiprojecttest01.dev.labs.internal/', verify=False)
 
         assert r.status_code == 200
         assert r.text
 
     @pytest.mark.skipif(REQUESTS_SUPPORTS_SSL_CONTEXT, reason="Will not raise exc")
     def test_requires_new_enough_requests(self):
         with pytest.raises(exc.VersionMismatchError):
-            X509Adapter()      
+            X509Adapter()
```

### Comparing `requests-toolbelt-0.9.1/tests/test_multipart_decoder.py` & `requests-toolbelt-1.0.0/tests/test_multipart_decoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # -*- coding: utf-8 -*-
 import io
 import sys
 import unittest
-import mock
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 import pytest
 import requests
 from requests_toolbelt.multipart.decoder import BodyPart
 from requests_toolbelt.multipart.decoder import (
     ImproperBodyPartContentException
 )
 from requests_toolbelt.multipart.decoder import MultipartDecoder
@@ -124,15 +127,15 @@
 
         parts_iter = zip(self.decoded_1.parts, self.sample_1)
         assert all(parts_equal(part, sample) for part, sample in parts_iter)
 
     def test_header_of_parts(self):
         def parts_header_equal(part, sample):
             return part.headers[b'Content-Disposition'] == encode_with(
-                'form-data; name="{0}"'.format(sample[0]), 'utf-8'
+                'form-data; name="{}"'.format(sample[0]), 'utf-8'
             )
 
         parts_iter = zip(self.decoded_1.parts, self.sample_1)
         assert all(
             parts_header_equal(part, sample)
             for part, sample in parts_iter
         )
@@ -184,8 +187,7 @@
         assert decoder_2.content_type == response.headers['content-type']
         assert (
             decoder_2.parts[0].content == b'Body 1, Line 1\r\nBody 1, Line 2'
         )
         assert decoder_2.parts[0].headers[b'Header-1'] == b'Header-Value-1'
         assert len(decoder_2.parts[1].headers) == 0
         assert decoder_2.parts[1].content == b'Body 2, Line 1'
-
```

### Comparing `requests-toolbelt-0.9.1/tests/threaded/test_pool.py` & `requests-toolbelt-1.0.0/tests/threaded/test_pool.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 """Module containing the tests for requests_toolbelt.threaded.pool."""
 try:
     import queue  # Python 3
 except ImportError:
     import Queue as queue
 import unittest
 
-import mock
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 import pytest
 
 from requests_toolbelt.threaded import pool
 from requests_toolbelt.threaded import thread
 
 
 class TestPool(unittest.TestCase):
@@ -22,46 +25,51 @@
             pool.Pool(None, num_processes=0)
 
         with pytest.raises(ValueError):
             pool.Pool(None, num_processes=-1)
 
     def test_number_of_processes_can_be_arbitrary(self):
         """Show that the number of processes can be set."""
-        p = pool.Pool(None, num_processes=100)
+        job_queue = queue.Queue()
+        p = pool.Pool(job_queue, num_processes=100)
         assert p._processes == 100
         assert len(p._pool) == 100
 
-        p = pool.Pool(None, num_processes=1)
+        job_queue = queue.Queue()
+        p = pool.Pool(job_queue, num_processes=1)
         assert p._processes == 1
         assert len(p._pool) == 1
 
     def test_initializer_is_called(self):
         """Ensure that the initializer function is called."""
+        job_queue = queue.Queue()
         initializer = mock.MagicMock()
-        pool.Pool(None, num_processes=1, initializer=initializer)
+        pool.Pool(job_queue, num_processes=1, initializer=initializer)
         assert initializer.called is True
         initializer.assert_called_once_with(mock.ANY)
 
     def test_auth_generator_is_called(self):
         """Ensure that the auth_generator function is called."""
+        job_queue = queue.Queue()
         auth_generator = mock.MagicMock()
-        pool.Pool(None, num_processes=1, auth_generator=auth_generator)
+        pool.Pool(job_queue, num_processes=1, auth_generator=auth_generator)
         assert auth_generator.called is True
         auth_generator.assert_called_once_with(mock.ANY)
 
     def test_session_is_called(self):
         """Ensure that the session function is called."""
+        job_queue = queue.Queue()
         session = mock.MagicMock()
-        pool.Pool(None, num_processes=1, session=session)
+        pool.Pool(job_queue, num_processes=1, session=session)
         assert session.called is True
         session.assert_called_once_with()
 
     def test_from_exceptions_populates_a_queue(self):
         """Ensure a Queue is properly populated from exceptions."""
-        urls = ["https://httpbin.org/get?n={0}".format(n) for n in range(5)]
+        urls = ["https://httpbin.org/get?n={}".format(n) for n in range(5)]
         Exc = pool.ThreadException
         excs = (Exc({'method': 'GET', 'url': url}, None) for url in urls)
 
         job_queue = mock.MagicMock()
         with mock.patch.object(queue, 'Queue', return_value=job_queue):
             with mock.patch.object(thread, 'SessionThread'):
                 pool.Pool.from_exceptions(excs)
@@ -70,15 +78,15 @@
         assert job_queue.put.mock_calls == [
             mock.call({'method': 'GET', 'url': url})
             for url in urls
         ]
 
     def test_from_urls_constructs_get_requests(self):
         """Ensure a Queue is properly populated from an iterable of urls."""
-        urls = ["https://httpbin.org/get?n={0}".format(n) for n in range(5)]
+        urls = ["https://httpbin.org/get?n={}".format(n) for n in range(5)]
 
         job_queue = mock.MagicMock()
         with mock.patch.object(queue, 'Queue', return_value=job_queue):
             with mock.patch.object(thread, 'SessionThread'):
                 pool.Pool.from_urls(urls)
 
         assert job_queue.put.call_count == 5
@@ -91,15 +99,15 @@
         """Ensure a Queue is properly populated from an iterable of urls."""
         def merge(*args):
             final = {}
             for d in args:
                 final.update(d)
             return final
 
-        urls = ["https://httpbin.org/get?n={0}".format(n) for n in range(5)]
+        urls = ["https://httpbin.org/get?n={}".format(n) for n in range(5)]
 
         kwargs = {'stream': True, 'headers': {'Accept': 'application/json'}}
         job_queue = mock.MagicMock()
         with mock.patch.object(queue, 'Queue', return_value=job_queue):
             with mock.patch.object(thread, 'SessionThread'):
                 pool.Pool.from_urls(urls, kwargs)
```

### Comparing `requests-toolbelt-0.9.1/tests/threaded/test_thread.py` & `requests-toolbelt-1.0.0/tests/threaded/test_thread.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,26 +3,31 @@
     import queue  # Python 3
 except ImportError:
     import Queue as queue
 import threading
 import unittest
 import uuid
 
-import mock
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 import requests.exceptions
 
 from requests_toolbelt.threaded import thread
 
 
 def _make_mocks():
     return (mock.MagicMock() for _ in range(4))
 
 
 def _initialize_a_session_thread(session=None, job_queue=None,
                                  response_queue=None, exception_queue=None):
+    if job_queue is None:
+        job_queue = queue.Queue()
     with mock.patch.object(threading, 'Thread') as Thread:
         thread_instance = mock.MagicMock()
         Thread.return_value = thread_instance
         st = thread.SessionThread(
             initialized_session=session,
             job_queue=job_queue,
             response_queue=response_queue,
@@ -48,18 +53,19 @@
         Thread.assert_called_once_with(target=st._make_request, name='test')
         assert thread_instance.daemon is True
         assert thread_instance._state is 0
         thread_instance.start.assert_called_once_with()
 
     def test_is_alive_proxies_to_worker(self):
         """Test that we proxy the is_alive method to the Thread."""
+        job_queue = queue.Queue()
         with mock.patch.object(threading, 'Thread') as Thread:
             thread_instance = mock.MagicMock()
             Thread.return_value = thread_instance
-            st = thread.SessionThread(None, None, None, None)
+            st = thread.SessionThread(None, job_queue, None, None)
 
         st.is_alive()
         thread_instance.is_alive.assert_called_once_with()
 
     def test_join_proxies_to_worker(self):
         """Test that we proxy the join method to the Thread."""
         st, thread_instance, _ = _initialize_a_session_thread()
```

### Comparing `requests-toolbelt-0.9.1/tests/threaded/test_api.py` & `requests-toolbelt-1.0.0/tests/threaded/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """Module containing tests for requests_toolbelt.threaded API."""
 
-import mock
+try:
+    from unittest import mock
+except ImportError:
+    import mock
 import pytest
 
 from requests_toolbelt._compat import queue
 from requests_toolbelt import threaded
 
 
 def test_creates_a_pool_for_the_user():
```

### Comparing `requests-toolbelt-0.9.1/setup.py` & `requests-toolbelt-1.0.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -40,29 +40,41 @@
 
 setup(
     name="requests-toolbelt",
     version=__version__,
     description="A utility belt for advanced users of python-requests",
     long_description="\n\n".join([open("README.rst").read(),
                                   open("HISTORY.rst").read()]),
+    long_description_content_type="text/x-rst",
     license='Apache 2.0',
     author='Ian Cordasco, Cory Benfield',
     author_email="graffatcolmingov@gmail.com",
-    url="https://toolbelt.readthedocs.org",
+    url="https://toolbelt.readthedocs.io/",
+    project_urls={
+        "Changelog": "https://github.com/requests/toolbelt/blob/master/HISTORY.rst",
+        "Source": "https://github.com/requests/toolbelt",
+    },
     packages=packages,
     package_data={'': ['LICENSE', 'AUTHORS.rst']},
     include_package_data=True,
+    python_requires='>=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*',
     install_requires=['requests>=2.0.1,<3.0.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'License :: OSI Approved :: Apache Software License',
         'Intended Audience :: Developers',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy',
     ],
 )
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/utils/deprecated.py` & `requests-toolbelt-1.0.0/requests_toolbelt/utils/deprecated.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/utils/formdata.py` & `requests-toolbelt-1.0.0/requests_toolbelt/utils/formdata.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/utils/user_agent.py` & `requests-toolbelt-1.0.0/requests_toolbelt/utils/user_agent.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/utils/dump.py` & `requests-toolbelt-1.0.0/requests_toolbelt/utils/dump.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     if request.body:
         if isinstance(request.body, compat.basestring):
             bytearr.extend(prefix + _coerce_to_bytes(request.body))
         else:
             # In the event that the body is a file-like object, let's not try
             # to read everything into memory.
             bytearr.extend(b'<< Request body is not a string-like type >>')
+        bytearr.extend(b'\r\n')
     bytearr.extend(b'\r\n')
 
 
 def _dump_response_data(response, prefixes, bytearr):
     prefix = prefixes.response
     # Let's interact almost entirely with urllib3's response
     raw = response.raw
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/streaming_iterator.py` & `requests-toolbelt-1.0.0/requests_toolbelt/streaming_iterator.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/adapters/ssl.py` & `requests-toolbelt-1.0.0/requests_toolbelt/adapters/ssl.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/adapters/x509.py` & `requests-toolbelt-1.0.0/requests_toolbelt/adapters/x509.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,30 @@
 from cryptography.hazmat.primitives.serialization import Encoding
 from cryptography.hazmat.backends import default_backend
 
 from datetime import datetime
 from requests.adapters import HTTPAdapter
 import requests
 
-from .._compat import PyOpenSSLContext
 from .. import exceptions as exc
 
 """
 importing the protocol constants from _ssl instead of ssl because only the
 constants are needed and to handle issues caused by importing from ssl on
 the 2.7.x line.
 """
 try:
     from _ssl import PROTOCOL_TLS as PROTOCOL
 except ImportError:
     from _ssl import PROTOCOL_SSLv23 as PROTOCOL
 
 
+PyOpenSSLContext = None
+
+
 class X509Adapter(HTTPAdapter):
     r"""Adapter for use with X.509 certificates.
 
     Provides an interface for Requests sessions to contact HTTPS urls and
     authenticate  with an X.509 cert by implementing the Transport Adapter
     interface. This class will need to be manually instantiated and mounted
     to the session
@@ -77,14 +79,15 @@
       >>> s = requests.Session()
       >>> a = X509Adapter(max_retries=3,
                 cert_bytes=b'...', pk_bytes=b'...', encoding='...'
       >>> s.mount('https://', a)
     """
 
     def __init__(self, *args, **kwargs):
+        self._import_pyopensslcontext()
         self._check_version()
         cert_bytes = kwargs.pop('cert_bytes', None)
         pk_bytes = kwargs.pop('pk_bytes', None)
         password = kwargs.pop('password', None)
         encoding = kwargs.pop('encoding', Encoding.PEM)
 
         password_bytes = None
@@ -114,32 +117,47 @@
         return super(X509Adapter, self).init_poolmanager(*args, **kwargs)
 
     def proxy_manager_for(self, *args, **kwargs):
         if self.ssl_context:
             kwargs['ssl_context'] = self.ssl_context
         return super(X509Adapter, self).proxy_manager_for(*args, **kwargs)
 
+    def _import_pyopensslcontext(self):
+        global PyOpenSSLContext
+
+        if requests.__build__ < 0x021200:
+            PyOpenSSLContext = None
+        else:
+            try:
+                from requests.packages.urllib3.contrib.pyopenssl \
+                        import PyOpenSSLContext
+            except ImportError:
+                try:
+                    from urllib3.contrib.pyopenssl import PyOpenSSLContext
+                except ImportError:
+                    PyOpenSSLContext = None
+
     def _check_version(self):
         if PyOpenSSLContext is None:
             raise exc.VersionMismatchError(
                 "The X509Adapter requires at least Requests 2.12.0 to be "
-                "installed. Version {0} was found instead.".format(
+                "installed. Version {} was found instead.".format(
                     requests.__version__
                 )
             )
 
 
 def check_cert_dates(cert):
     """Verify that the supplied client cert is not invalid."""
 
     now = datetime.utcnow()
     if cert.not_valid_after < now or cert.not_valid_before > now:
         raise ValueError('Client certificate expired: Not After: '
-                         '{0:%Y-%m-%d %H:%M:%SZ} '
-                         'Not Before: {1:%Y-%m-%d %H:%M:%SZ}'
+                         '{:%Y-%m-%d %H:%M:%SZ} '
+                         'Not Before: {:%Y-%m-%d %H:%M:%SZ}'
                          .format(cert.not_valid_after, cert.not_valid_before))
 
 
 def create_ssl_context(cert_byes, pk_bytes, password=None,
                        encoding=Encoding.PEM):
     """Create an SSL Context with the supplied cert/password.
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/adapters/source.py` & `requests-toolbelt-1.0.0/requests_toolbelt/adapters/source.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/adapters/fingerprint.py` & `requests-toolbelt-1.0.0/requests_toolbelt/adapters/fingerprint.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/adapters/host_header_ssl.py` & `requests-toolbelt-1.0.0/requests_toolbelt/adapters/host_header_ssl.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/adapters/socket_options.py` & `requests-toolbelt-1.0.0/requests_toolbelt/adapters/socket_options.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -80,17 +80,17 @@
     - ``IPPROTO_TCP`` ``TCP_KEEPINTVL`` 20 - Sets the keep alive interval
     - ``IPPROTO_TCP`` ``TCP_KEEPCNT`` 5 - Sets the number of keep alive probes
     - ``IPPROTO_TCP`` ``TCP_KEEPIDLE`` 60 - Sets the keep alive time if the
       socket library has the ``TCP_KEEPIDLE`` constant
 
     The latter three can be overridden by keyword arguments (respectively):
 
-    - ``idle``
     - ``interval``
     - ``count``
+    - ``idle``
 
     You can use this adapter like so::
 
        >>> from requests_toolbelt.adapters import socket_options
        >>> tcp = socket_options.TCPKeepAliveAdapter(idle=120, interval=10)
        >>> s = requests.Session()
        >>> s.mount('http://', tcp)
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/downloadutils/stream.py` & `requests-toolbelt-1.0.0/requests_toolbelt/downloadutils/stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 """Utilities for dealing with streamed requests."""
-import collections
 import os.path
 import re
 
 from .. import exceptions as exc
 
 # Regular expressions stolen from werkzeug/http.py
 # cd2c97bb0a076da2322f11adce0b2731f9193396 L62-L64
@@ -127,15 +126,15 @@
         import requests
         from requests_toolbelt.downloadutils import stream
 
         with open('myfile', 'wb') as fd:
             r = requests.get(url, stream=True)
             filename = stream.stream_response_to_file(r, path=fd)
 
-        print('{0} saved to {1}'.format(url, filename))
+        print('{} saved to {}'.format(url, filename))
 
     .. code-block:: python
 
         import io
         import requests
         from requests_toolbelt.downloadutils import stream
 
@@ -154,15 +153,15 @@
     :returns: The name of the file, if one can be determined, else None
     :rtype: str
     :raises: :class:`requests_toolbelt.exceptions.StreamingError`
     """
     pre_opened = False
     fd = None
     filename = None
-    if path and isinstance(getattr(path, 'write', None), collections.Callable):
+    if path and callable(getattr(path, 'write', None)):
         pre_opened = True
         fd = path
         filename = getattr(fd, 'name', None)
     else:
         filename = get_download_file_path(response, path)
         if os.path.exists(filename):
             raise exc.StreamingError("File already exists: %s" % filename)
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/downloadutils/tee.py` & `requests-toolbelt-1.0.0/requests_toolbelt/downloadutils/tee.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/_compat.py` & `requests-toolbelt-1.0.0/requests_toolbelt/_compat.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,34 +37,14 @@
     timeout = None
 else:
     try:
         from requests.packages.urllib3.util import timeout
     except ImportError:
         from urllib3.util import timeout
 
-if requests.__build__ < 0x021000:
-    gaecontrib = None
-else:
-    try:
-        from requests.packages.urllib3.contrib import appengine as gaecontrib
-    except ImportError:
-        from urllib3.contrib import appengine as gaecontrib
-
-if requests.__build__ < 0x021200:
-    PyOpenSSLContext = None
-else:
-    try:
-        from requests.packages.urllib3.contrib.pyopenssl \
-                import PyOpenSSLContext
-    except ImportError:
-        try:
-            from urllib3.contrib.pyopenssl import PyOpenSSLContext
-        except ImportError:
-            PyOpenSSLContext = None
-
 PY3 = sys.version_info > (3, 0)
 
 if PY3:
     from collections.abc import Mapping, MutableMapping
     import queue
     from urllib.parse import urlencode, urljoin
 else:
@@ -139,16 +119,16 @@
         return key.lower() in self._container
 
     def __eq__(self, other):
         if not isinstance(other, Mapping) and not hasattr(other, 'keys'):
             return False
         if not isinstance(other, type(self)):
             other = type(self)(other)
-        return (dict((k.lower(), v) for k, v in self.itermerged()) ==
-                dict((k.lower(), v) for k, v in other.itermerged()))
+        return ({k.lower(): v for k, v in self.itermerged()} ==
+                {k.lower(): v for k, v in other.itermerged()})
 
     def __ne__(self, other):
         return not self.__eq__(other)
 
     if not PY3:  # Python 2
         iterkeys = MutableMapping.iterkeys
         itervalues = MutableMapping.itervalues
@@ -314,11 +294,9 @@
     'fields',
     'filepost',
     'poolmanager',
     'timeout',
     'HTTPHeaderDict',
     'queue',
     'urlencode',
-    'gaecontrib',
     'urljoin',
-    'PyOpenSSLContext',
 )
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/multipart/encoder.py` & `requests-toolbelt-1.0.0/requests_toolbelt/multipart/encoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     .. code-block:: python
 
         import requests
         from requests_toolbelt import MultipartEncoder
 
         encoder = MultipartEncoder({'field': 'value',
-                                    'other_field', 'other_value'})
+                                    'other_field': 'other_value'})
         r = requests.post('https://httpbin.org/post', data=encoder,
                           headers={'Content-Type': encoder.content_type})
 
     If you do not need to take advantage of streaming the post body, you can
     also do:
 
     .. code-block:: python
@@ -85,15 +85,15 @@
     """
 
     def __init__(self, fields, boundary=None, encoding='utf-8'):
         #: Boundary value either passed in by the user or created
         self.boundary_value = boundary or uuid4().hex
 
         # Computed boundary
-        self.boundary = '--{0}'.format(self.boundary_value)
+        self.boundary = '--{}'.format(self.boundary_value)
 
         #: Encoding of the data being passed in
         self.encoding = encoding
 
         # Pre-encoded boundary
         self._encoded_boundary = b''.join([
             encode_with(self.boundary, self.encoding),
@@ -144,15 +144,15 @@
         .. _bug #80:
             https://github.com/requests/toolbelt/issues/80
         """
         # If _len isn't already calculated, calculate, return, and set it
         return self._len or self._calculate_length()
 
     def __repr__(self):
-        return '<MultipartEncoder: {0!r}>'.format(self.fields)
+        return '<MultipartEncoder: {!r}>'.format(self.fields)
 
     def _calculate_length(self):
         """
         This uses the parts to calculate the length of the body.
 
         This returns the calculated length so __len__ can be lazy.
         """
@@ -269,15 +269,15 @@
     def _write_headers(self, headers):
         """Write the current part's headers to the buffer."""
         return self._write(encode_with(headers, self.encoding))
 
     @property
     def content_type(self):
         return str(
-            'multipart/form-data; boundary={0}'.format(self.boundary_value)
+            'multipart/form-data; boundary={}'.format(self.boundary_value)
             )
 
     def to_string(self):
         """Return the entirety of the data in the encoder.
 
         .. note::
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/multipart/decoder.py` & `requests-toolbelt-1.0.0/requests_toolbelt/multipart/decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     a bytestring into a tuple of ``Response``-like ``BodyPart`` objects.
 
     The basic usage is::
 
         import requests
         from requests_toolbelt import MultipartDecoder
 
-        response = request.get(url)
+        response = requests.get(url)
         decoder = MultipartDecoder.from_response(response)
         for part in decoder.parts:
             print(part.headers['content-type'])
 
     If the multipart content is not from a response, basic usage is::
 
         from requests_toolbelt import MultipartDecoder
@@ -111,15 +111,15 @@
         self._parse_body(content)
 
     def _find_boundary(self):
         ct_info = tuple(x.strip() for x in self.content_type.split(';'))
         mimetype = ct_info[0]
         if mimetype.split('/')[0].lower() != 'multipart':
             raise NonMultipartContentTypeException(
-                "Unexpected mimetype in content-type: '{0}'".format(mimetype)
+                "Unexpected mimetype in content-type: '{}'".format(mimetype)
             )
         for item in ct_info[1:]:
             attr, value = _split_on_find(
                 item,
                 '='
             )
             if attr.lower() == 'boundary':
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/multipart/__init__.py` & `requests-toolbelt-1.0.0/requests_toolbelt/multipart/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 requests_toolbelt.multipart
 ===========================
 
-See http://toolbelt.rtfd.org/ for documentation
+See https://toolbelt.readthedocs.io/ for documentation
 
 :copyright: (c) 2014 by Ian Cordasco and Cory Benfield
 :license: Apache v2.0, see LICENSE for more details
 """
 
 from .encoder import MultipartEncoder, MultipartEncoderMonitor
 from .decoder import MultipartDecoder
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/auth/http_proxy_digest.py` & `requests-toolbelt-1.0.0/requests_toolbelt/auth/http_proxy_digest.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
             elif not self._pat.match(s_auth):
                 return r
 
             self.chal = utils.parse_dict_header(
                 self._pat.sub('', s_auth, count=1))
 
             # if we present the user/passwd and still get rejected
-            # http://tools.ietf.org/html/rfc2617#section-3.2.1
+            # https://tools.ietf.org/html/rfc2617#section-3.2.1
             if ('Proxy-Authorization' in r.request.headers and
                     'stale' in self.chal):
                 if self.chal['stale'].lower() == 'true':  # try again
                     self.stale_rejects += 1
                 # wrong user/passwd
                 elif self.chal['stale'].lower() == 'false':
                     raise IOError("User or password is invalid")
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/auth/_digest_auth_compat.py` & `requests-toolbelt-1.0.0/requests_toolbelt/auth/_digest_auth_compat.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/auth/handler.py` & `requests-toolbelt-1.0.0/requests_toolbelt/auth/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self._make_uniform()
 
     def __call__(self, request):
         auth = self.get_strategy_for(request.url)
         return auth(request)
 
     def __repr__(self):
-        return '<AuthHandler({0!r})>'.format(self.strategies)
+        return '<AuthHandler({!r})>'.format(self.strategies)
 
     def _make_uniform(self):
         existing_strategies = list(self.strategies.items())
         self.strategies = {}
 
         for (k, v) in existing_strategies:
             self.add_strategy(k, v)
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/auth/guess.py` & `requests-toolbelt-1.0.0/requests_toolbelt/auth/guess.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/sessions.py` & `requests-toolbelt-1.0.0/requests_toolbelt/sessions.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,45 +2,57 @@
 
 from ._compat import urljoin
 
 
 class BaseUrlSession(requests.Session):
     """A Session with a URL that all requests will use as a base.
 
-    Let's start by looking at an example:
+    Let's start by looking at a few examples:
 
     .. code-block:: python
 
         >>> from requests_toolbelt import sessions
         >>> s = sessions.BaseUrlSession(
         ...     base_url='https://example.com/resource/')
-        >>> r = s.get('sub-resource/' params={'foo': 'bar'})
+        >>> r = s.get('sub-resource/', params={'foo': 'bar'})
         >>> print(r.request.url)
         https://example.com/resource/sub-resource/?foo=bar
 
     Our call to the ``get`` method will make a request to the URL passed in
     when we created the Session and the partial resource name we provide.
+    We implement this by overriding the ``request`` method of the Session.
 
-    We implement this by overriding the ``request`` method so most uses of a
-    Session are covered. (This, however, precludes the use of PreparedRequest
-    objects).
+    Likewise, we override the ``prepare_request`` method so you can construct
+    a PreparedRequest in the same way:
+
+    .. code-block:: python
+
+        >>> from requests import Request
+        >>> from requests_toolbelt import sessions
+        >>> s = sessions.BaseUrlSession(
+        ...     base_url='https://example.com/resource/')
+        >>> request = Request(method='GET', url='sub-resource/')
+        >>> prepared_request = s.prepare_request(request)
+        >>> r = s.send(prepared_request)
+        >>> print(r.request.url)
+        https://example.com/resource/sub-resource
 
     .. note::
 
         The base URL that you provide and the path you provide are **very**
         important.
 
     Let's look at another *similar* example
 
     .. code-block:: python
 
         >>> from requests_toolbelt import sessions
         >>> s = sessions.BaseUrlSession(
         ...     base_url='https://example.com/resource/')
-        >>> r = s.get('/sub-resource/' params={'foo': 'bar'})
+        >>> r = s.get('/sub-resource/', params={'foo': 'bar'})
         >>> print(r.request.url)
         https://example.com/sub-resource/?foo=bar
 
     The key difference here is that we called ``get`` with ``/sub-resource/``,
     i.e., there was a leading ``/``. This changes how we create the URL
     because we rely on :mod:`urllib.parse.urljoin`.
 
@@ -61,10 +73,17 @@
     def request(self, method, url, *args, **kwargs):
         """Send the request after generating the complete URL."""
         url = self.create_url(url)
         return super(BaseUrlSession, self).request(
             method, url, *args, **kwargs
         )
 
+    def prepare_request(self, request, *args, **kwargs):
+        """Prepare the request after generating the complete URL."""
+        request.url = self.create_url(request.url)
+        return super(BaseUrlSession, self).prepare_request(
+            request, *args, **kwargs
+        )
+
     def create_url(self, url):
         """Create the URL based off this partial path."""
         return urljoin(self.base_url, url)
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/__init__.py` & `requests-toolbelt-1.0.0/requests_toolbelt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 """
 requests-toolbelt
 =================
 
-See http://toolbelt.rtfd.org/ for documentation
+See https://toolbelt.readthedocs.io/ for documentation
 
 :copyright: (c) 2014 by Ian Cordasco and Cory Benfield
 :license: Apache v2.0, see LICENSE for more details
 """
 
 from .adapters import SSLAdapter, SourceAddressAdapter
 from .auth.guess import GuessAuth
@@ -18,15 +18,15 @@
 from .streaming_iterator import StreamingIterator
 from .utils.user_agent import user_agent
 
 __title__ = 'requests-toolbelt'
 __authors__ = 'Ian Cordasco, Cory Benfield'
 __license__ = 'Apache v2.0'
 __copyright__ = 'Copyright 2014 Ian Cordasco, Cory Benfield'
-__version__ = '0.9.1'
+__version__ = '1.0.0'
 __version_info__ = tuple(int(i) for i in __version__.split('.'))
 
 __all__ = [
     'GuessAuth', 'MultipartEncoder', 'MultipartEncoderMonitor',
     'MultipartDecoder', 'SSLAdapter', 'SourceAddressAdapter',
     'StreamingIterator', 'user_agent', 'ImproperBodyPartContentException',
     'NonMultipartContentTypeException', '__title__', '__authors__',
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/threaded/thread.py` & `requests-toolbelt-1.0.0/requests_toolbelt/threaded/thread.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/threaded/pool.py` & `requests-toolbelt-1.0.0/requests_toolbelt/threaded/pool.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt/threaded/__init__.py` & `requests-toolbelt-1.0.0/requests_toolbelt/threaded/__init__.py`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/CODE_OF_CONDUCT.rst` & `requests-toolbelt-1.0.0/CODE_OF_CONDUCT.rst`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 Instances of abusive, harassing, or otherwise unacceptable behavior may
 be reported by contacting a project maintainer at graffatcolmingov@gmail.com.
 All complaints will be reviewed and investigated and will
 result in a response that is deemed necessary and appropriate to the
 circumstances. Maintainers are obligated to maintain confidentiality
 with regard to the reporter of an incident.
 
-This Code of Conduct is adapted from the `Contributor Covenant`_, version 
-1.3.0, available at http://contributor-covenant.org/version/1/3/0/
+This Code of Conduct is adapted from the `Contributor Covenant`_, version
+1.3.0, available at https://www.contributor-covenant.org/version/1/3/0/
 
-.. _Contributor Covenant: http://contributor-covenant.org
+.. _Contributor Covenant: https://www.contributor-covenant.org/
 
 ..
     Re-formatted to reStructuredText from
     https://raw.githubusercontent.com/CoralineAda/contributor_covenant/master/CODE_OF_CONDUCT.md
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt.egg-info/SOURCES.txt` & `requests-toolbelt-1.0.0/requests_toolbelt.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 requests_toolbelt/streaming_iterator.py
 requests_toolbelt.egg-info/PKG-INFO
 requests_toolbelt.egg-info/SOURCES.txt
 requests_toolbelt.egg-info/dependency_links.txt
 requests_toolbelt.egg-info/requires.txt
 requests_toolbelt.egg-info/top_level.txt
 requests_toolbelt/adapters/__init__.py
-requests_toolbelt/adapters/appengine.py
 requests_toolbelt/adapters/fingerprint.py
 requests_toolbelt/adapters/host_header_ssl.py
 requests_toolbelt/adapters/socket_options.py
 requests_toolbelt/adapters/source.py
 requests_toolbelt/adapters/ssl.py
 requests_toolbelt/adapters/x509.py
 requests_toolbelt/auth/__init__.py
@@ -62,15 +61,14 @@
 requests_toolbelt/utils/__init__.py
 requests_toolbelt/utils/deprecated.py
 requests_toolbelt/utils/dump.py
 requests_toolbelt/utils/formdata.py
 requests_toolbelt/utils/user_agent.py
 tests/__init__.py
 tests/conftest.py
-tests/test_appengine_adapter.py
 tests/test_auth.py
 tests/test_auth_handler.py
 tests/test_downloadutils.py
 tests/test_dump.py
 tests/test_fingerprintadapter.py
 tests/test_forgetfulcookiejar.py
 tests/test_formdata.py
@@ -92,14 +90,14 @@
 tests/cassettes/httpbin_guess_auth_basic.json
 tests/cassettes/httpbin_guess_auth_digest.json
 tests/cassettes/httpbin_guess_auth_none.json
 tests/cassettes/klevas_vu_lt_ssl3.json
 tests/cassettes/redirect_request_for_dump_all.json
 tests/cassettes/simple_get_request.json
 tests/cassettes/stream_response_to_file.json
+tests/cassettes/stream_response_without_content_length_to_file.json
 tests/cassettes/test_x509_adapter_der.json
 tests/cassettes/test_x509_adapter_pem.json
-tests/certs/test_cert.p12
 tests/threaded/__init__.py
 tests/threaded/test_api.py
 tests/threaded/test_pool.py
 tests/threaded/test_thread.py
```

### Comparing `requests-toolbelt-0.9.1/requests_toolbelt.egg-info/PKG-INFO` & `requests-toolbelt-1.0.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,479 +1,520 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: requests-toolbelt
-Version: 0.9.1
+Version: 1.0.0
 Summary: A utility belt for advanced users of python-requests
-Home-page: https://toolbelt.readthedocs.org
+Home-page: https://toolbelt.readthedocs.io/
 Author: Ian Cordasco, Cory Benfield
 Author-email: graffatcolmingov@gmail.com
 License: Apache 2.0
-Description: The Requests Toolbelt
-        =====================
-        
-        This is just a collection of utilities for `python-requests`_, but don't 
-        really belong in ``requests`` proper. The minimum tested requests version is 
-        ``2.1.0``. In reality, the toolbelt should work with ``2.0.1`` as well, but 
-        some idiosyncracies prevent effective or sane testing on that version.
-        
-        ``pip install requests-toolbelt`` to get started!
-        
-        
-        multipart/form-data Encoder
-        ---------------------------
-        
-        The main attraction is a streaming multipart form-data object, ``MultipartEncoder``.
-        Its API looks like this:
-        
-        .. code-block:: python
-        
-            from requests_toolbelt import MultipartEncoder
-            import requests
-        
-            m = MultipartEncoder(
-                fields={'field0': 'value', 'field1': 'value',
-                        'field2': ('filename', open('file.py', 'rb'), 'text/plain')}
-                )
-        
-            r = requests.post('http://httpbin.org/post', data=m,
-                              headers={'Content-Type': m.content_type})
-        
-        
-        You can also use ``multipart/form-data`` encoding for requests that don't
-        require files:
-        
-        .. code-block:: python
-        
-            from requests_toolbelt import MultipartEncoder
-            import requests
-        
-            m = MultipartEncoder(fields={'field0': 'value', 'field1': 'value'})
-        
-            r = requests.post('http://httpbin.org/post', data=m,
-                              headers={'Content-Type': m.content_type})
-        
-        
-        Or, you can just create the string and examine the data:
-        
-        .. code-block:: python
-        
-            # Assuming `m` is one of the above
-            m.to_string()  # Always returns unicode
-        
-        
-        User-Agent constructor
-        ----------------------
-        
-        You can easily construct a requests-style ``User-Agent`` string::
-        
-            from requests_toolbelt import user_agent
-        
-            headers = {
-                'User-Agent': user_agent('my_package', '0.0.1')
-                }
-        
-            r = requests.get('https://api.github.com/users', headers=headers)
-        
-        
-        SSLAdapter
-        ----------
-        
-        The ``SSLAdapter`` was originally published on `Cory Benfield's blog`_. 
-        This adapter allows the user to choose one of the SSL protocols made available 
-        in Python's ``ssl`` module for outgoing HTTPS connections:
-        
-        .. code-block:: python
-        
-            from requests_toolbelt import SSLAdapter
-            import requests
-            import ssl
-        
-            s = requests.Session()
-            s.mount('https://', SSLAdapter(ssl.PROTOCOL_TLSv1))
-        
-        cookies/ForgetfulCookieJar
-        --------------------------
-        
-        The ``ForgetfulCookieJar`` prevents a particular requests session from storing 
-        cookies:
-        
-        .. code-block:: python
-        
-            from requests_toolbelt.cookies.forgetful import ForgetfulCookieJar
-        
-            session = requests.Session()
-            session.cookies = ForgetfulCookieJar()
-        
-        Known Issues
-        ------------
-        
-        On Python 3.3.0 and 3.3.1, the standard library's ``http`` module will fail
-        when passing an instance of the ``MultipartEncoder``. This is fixed in later
-        minor releases of Python 3.3. Please consider upgrading to a later minor
-        version or Python 3.4. *There is absolutely nothing this library can do to
-        work around that bug.*
-        
-        Contributing
-        ------------
-        
-        Please read the `suggested workflow
-        <https://toolbelt.readthedocs.org/en/latest/contributing.html>`_ for
-        contributing to this project.
-        
-        Please report any bugs on the `issue tracker`_
-        
-        .. _Cory Benfield's blog: https://lukasa.co.uk/2013/01/Choosing_SSL_Version_In_Requests/
-        .. _python-requests: https://github.com/kennethreitz/requests
-        .. _issue tracker: https://github.com/requests/toolbelt/issues
-        
-        
-        History
-        =======
-        
-        0.9.1 -- 2019-01-29
-        -------------------
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Fix import of pyOpenSSL shim from urllib3 for PKCS12 adapter
-        
-        0.9.0 -- 2019-01-29
-        -------------------
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - Add X509 Adapter that can handle PKCS12 
-        - Add stateless solution for streaming files by MultipartEncoder from one host to another (in chunks)
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Update link to example
-        - Move import of ``ABCs`` from collections into version-specific part of
-          _compat module
-        - Fix backwards incompatibility in ``get_encodings_from_content``
-        - Correct callback documentation for ``MultipartEncoderMonitor``
-        - Fix bug when ``MultipartEncoder`` is asked to encode zero parts
-        - Correct the type of non string request body dumps
-        - Removed content from being stored in MultipartDecoder
-        - Fix bug by enabling support for contenttype with capital letters. 
-        - Coerce proxy URL to bytes before dumping request
-        - Avoid bailing out with exception upon empty response reason
-        - Corrected Pool documentation
-        - Corrected parentheses match in example usage
-        - Fix "oject" to "object" in ``MultipartEncoder``
-        - Fix URL for the project after the move 
-        - Add fix for OSX TCPKeepAliveAdapter
-        
-        Miscellaneous
-        ~~~~~~~~~~~~~
-        
-        - Remove py33 from testing and add Python 3.6 and nightly testing to the travis matrix.
-        
-        0.8.0 -- 2017-05-20
-        -------------------
-        
-        More information about this release can be found on the `0.8.0 milestone`_.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - Add ``UserAgentBuilder`` to provide more control over generated User-Agent
-          strings.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Include ``_validate_certificate`` in the lits of picked attributes on the
-          ``AppEngineAdapter``.
-        - Fix backwards incompatibility in ``get_encodings_from_content``
-        
-        .. _0.8.0 milestone:
-            https://github.com/requests/toolbelt/milestones/0.8.0
-        
-        0.7.1 -- 2017-02-13
-        -------------------
-        
-        More information about this release can be found on the `0.7.1 milestone`_.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Fixed monkey-patching for the AppEngineAdapter.
-        
-        - Make it easier to disable certificate verification when monkey-patching
-          AppEngine.
-        
-        - Handle ``multipart/form-data`` bodies without a trailing ``CRLF``.
-        
-        
-        .. links
-        .. _0.7.1 milestone:
-            https://github.com/requests/toolbelt/milestone/9
-        
-        0.7.0 -- 2016-07-21
-        -------------------
-        
-        More information about this release can be found on the `0.7.0 milestone`_.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - Add ``BaseUrlSession`` to allow developers to have a session that has a
-          "Base" URL. See the documentation for more details and examples.
-        
-        - Split the logic of ``stream_response_to_file`` into two separate functions:
-        
-          * ``get_download_file_path`` to generate the file name from the Response.
-        
-          * ``stream_response_to_file`` which will use ``get_download_file_path`` if
-            necessary
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Fixed the issue for people using *very* old versions of Requests where they
-          would see an ImportError from ``requests_toolbelt._compat`` when trying to
-          import ``connection``.
-        
-        
-        .. _0.7.0 milestone:
-            https://github.com/requests/toolbelt/milestones/0.7.0
-        
-        0.6.2 -- 2016-05-10
-        -------------------
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - When passing a timeout via Requests, it was not appropriately translated to
-          the timeout that the urllib3 code was expecting.
-        
-        0.6.1 -- 2016-05-05
-        -------------------
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Remove assertion about request URLs in the AppEngineAdapter.
-        
-        - Prevent pip from installing requests 3.0.0 when that is released until we
-          are ready to handle it.
-        
-        0.6.0 -- 2016-01-27
-        -------------------
-        
-        More information about this release can be found on the `0.6.0 milestone`_.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - Add ``AppEngineAdapter`` to support developers using Google's AppEngine
-          platform with Requests.
-        
-        - Add ``GuessProxyAuth`` class to support guessing between Basic and Digest
-          Authentication for proxies.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Ensure that proxies use the correct TLS version when using the
-          ``SSLAdapter``.
-        
-        - Fix an ``AttributeError`` when using the ``HTTPProxyDigestAuth`` class.
-        
-        Miscellaneous
-        ~~~~~~~~~~~~~
-        
-        - Drop testing support for Python 3.2. virtualenv and pip have stopped
-          supporting it meaning that it is harder to test for this with our CI
-          infrastructure. Moving forward we will make a best-effort attempt to
-          support 3.2 but will not test for it.
-        
-        
-        .. _0.6.0 milestone:
-            https://github.com/requests/toolbelt/milestones/0.6.0
-        
-        0.5.1 -- 2015-12-16
-        -------------------
-        
-        More information about this release can be found on the `0.5.1 milestone`_.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Now papers over the differences in requests' ``super_len`` function from
-          versions prior to 2.9.0 and versions 2.9.0 and later.
-        
-        
-        .. _0.5.1 milestone:
-            https://github.com/requests/toolbelt/milestones/0.5.1
-        
-        0.5.0 -- 2015-11-24
-        -------------------
-        
-        More information about this release can be found on the `milestone
-        <https://github.com/requests/toolbelt/issues?utf8=%E2%9C%93&q=is%3Aall+milestone%3A0.5+>`_
-        for 0.5.0.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - The ``tee`` submodule was added to ``requests_toolbelt.downloadutils``. It
-          allows you to iterate over the bytes of a response while also writing them
-          to a file. The ``tee.tee`` function, expects you to pass an open file
-          object, while ``tee.tee_to_file`` will use the provided file name to open
-          the file for you.
-        
-        - Added a new parameter to ``requests_toolbelt.utils.user_agent`` that allows
-          the user to specify additional items.
-        
-        - Added nested form-data helper,
-          ``requests_toolbelt.utils.formdata.urlencode``.
-        
-        - Added the ``ForgetfulCookieJar`` to ``requests_toolbelt.cookies``.
-        
-        - Added utilities for dumping the information about a request-response cycle
-          in ``requests_toolbelt.utils.dump``.
-        
-        - Implemented the API described in the ``requests_toolbelt.threaded`` module
-          docstring, i.e., added ``requests_toolbelt.threaded.map`` as an available
-          function.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Now papers over the API differences in versions of requests installed from
-          system packages versus versions of requests installed from PyPI.
-        
-        - Allow string types for ``SourceAddressAdapter``.
-        
-        0.4.0 -- 2015-04-03
-        -------------------
-        
-        For more information about this release, please see `milestone 0.4.0
-        <https://github.com/requests/toolbelt/issues?q=milestone%3A0.4>`_
-        on the project's page.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - A naive implemenation of a thread pool is now included in the toolbelt. See
-          the docs in ``docs/threading.rst`` or on `Read The Docs
-          <https://toolbelt.readthedocs.org>`_.
-        
-        - The ``StreamingIterator`` now accepts files (such as ``sys.stdin``) without
-          a specific length and will properly stream them.
-        
-        - The ``MultipartEncoder`` now accepts exactly the same format of fields as
-          requests' ``files`` parameter does. In other words, you can now also pass in
-          extra headers to add to a part in the body. You can also now specify a
-          custom ``Content-Type`` for a part.
-        
-        - An implementation of HTTP Digest Authentication for Proxies is now included.
-        
-        - A transport adapter that allows a user to specify a specific Certificate
-          Fingerprint is now included in the toolbelt.
-        
-        - A transport adapter that simplifies how users specify socket options is now
-          included.
-        
-        - A transport adapter that simplifies how users can specify TCP Keep-Alive
-          options is now included in the toolbelt.
-        
-        - Deprecated functions from ``requests.utils`` are now included and
-          maintained.
-        
-        - An authentication tool that allows users to specify how to authenticate to
-          several different domains at once is now included.
-        
-        - A function to save streamed responses to disk by analyzing the
-          ``Content-Disposition`` header is now included in the toolbelt.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - The ``MultipartEncoder`` will now allow users to upload files larger than
-          4GB on 32-bit systems.
-        
-        - The ``MultipartEncoder`` will now accept empty unicode strings for form
-          values.
-        
-        0.3.1 -- 2014-06-23
-        -------------------
-        
-        - Fix the fact that 0.3.0 bundle did not include the ``StreamingIterator``
-        
-        0.3.0 -- 2014-05-21
-        -------------------
-        
-        Bug Fixes
-        ~~~~~~~~~
-        
-        - Complete rewrite of ``MultipartEncoder`` fixes bug where bytes were lost in
-          uploads
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - ``MultipartDecoder`` to accept ``multipart/form-data`` response bodies and
-          parse them into an easy to use object.
-        
-        - ``SourceAddressAdapter`` to allow users to choose a local address to bind
-          connections to.
-        
-        - ``GuessAuth`` which accepts a username and password and uses the
-          ``WWW-Authenticate`` header to determine how to authenticate against a
-          server.
-        
-        - ``MultipartEncoderMonitor`` wraps an instance of the ``MultipartEncoder``
-          and keeps track of how many bytes were read and will call the provided
-          callback.
-        
-        - ``StreamingIterator`` will wrap an iterator and stream the upload instead of
-          chunk it, provided you also provide the length of the content you wish to
-          upload.
-        
-        0.2.0 -- 2014-02-24
-        -------------------
-        
-        - Add ability to tell ``MultipartEncoder`` which encoding to use. By default
-          it uses 'utf-8'.
-        
-        - Fix #10 - allow users to install with pip
-        
-        - Fix #9 - Fix ``MultipartEncoder#to_string`` so that it properly handles file
-          objects as fields
-        
-        0.1.2 -- 2014-01-19
-        -------------------
-        
-        - At some point during development we broke how we handle normal file objects.
-          Thanks to @konomae this is now fixed.
-        
-        0.1.1 -- 2014-01-19
-        -------------------
-        
-        - Handle ``io.BytesIO``-like objects better
-        
-        0.1.0 -- 2014-01-18
-        -------------------
-        
-        - Add initial implementation of the streaming ``MultipartEncoder``
-        
-        - Add initial implementation of the ``user_agent`` function
-        
-        - Add the ``SSLAdapter``
-        
-Platform: UNKNOWN
+Project-URL: Changelog, https://github.com/requests/toolbelt/blob/master/HISTORY.rst
+Project-URL: Source, https://github.com/requests/toolbelt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+The Requests Toolbelt
+=====================
+
+This is just a collection of utilities for `python-requests`_, but don't
+really belong in ``requests`` proper. The minimum tested requests version is
+``2.1.0``. In reality, the toolbelt should work with ``2.0.1`` as well, but
+some idiosyncracies prevent effective or sane testing on that version.
+
+``pip install requests-toolbelt`` to get started!
+
+
+multipart/form-data Encoder
+---------------------------
+
+The main attraction is a streaming multipart form-data object, ``MultipartEncoder``.
+Its API looks like this:
+
+.. code-block:: python
+
+    from requests_toolbelt import MultipartEncoder
+    import requests
+
+    m = MultipartEncoder(
+        fields={'field0': 'value', 'field1': 'value',
+                'field2': ('filename', open('file.py', 'rb'), 'text/plain')}
+        )
+
+    r = requests.post('http://httpbin.org/post', data=m,
+                      headers={'Content-Type': m.content_type})
+
+
+You can also use ``multipart/form-data`` encoding for requests that don't
+require files:
+
+.. code-block:: python
+
+    from requests_toolbelt import MultipartEncoder
+    import requests
+
+    m = MultipartEncoder(fields={'field0': 'value', 'field1': 'value'})
+
+    r = requests.post('http://httpbin.org/post', data=m,
+                      headers={'Content-Type': m.content_type})
+
+
+Or, you can just create the string and examine the data:
+
+.. code-block:: python
+
+    # Assuming `m` is one of the above
+    m.to_string()  # Always returns unicode
+
+
+User-Agent constructor
+----------------------
+
+You can easily construct a requests-style ``User-Agent`` string::
+
+    from requests_toolbelt import user_agent
+
+    headers = {
+        'User-Agent': user_agent('my_package', '0.0.1')
+        }
+
+    r = requests.get('https://api.github.com/users', headers=headers)
+
+
+SSLAdapter
+----------
+
+The ``SSLAdapter`` was originally published on `Cory Benfield's blog`_.
+This adapter allows the user to choose one of the SSL protocols made available
+in Python's ``ssl`` module for outgoing HTTPS connections:
+
+.. code-block:: python
+
+    from requests_toolbelt import SSLAdapter
+    import requests
+    import ssl
+
+    s = requests.Session()
+    s.mount('https://', SSLAdapter(ssl.PROTOCOL_TLSv1))
+
+cookies/ForgetfulCookieJar
+--------------------------
+
+The ``ForgetfulCookieJar`` prevents a particular requests session from storing
+cookies:
+
+.. code-block:: python
+
+    from requests_toolbelt.cookies.forgetful import ForgetfulCookieJar
+
+    session = requests.Session()
+    session.cookies = ForgetfulCookieJar()
+
+Contributing
+------------
+
+Please read the `suggested workflow
+<https://toolbelt.readthedocs.io/en/latest/contributing.html>`_ for
+contributing to this project.
+
+Please report any bugs on the `issue tracker`_
+
+.. _Cory Benfield's blog: https://lukasa.co.uk/2013/01/Choosing_SSL_Version_In_Requests/
+.. _python-requests: https://github.com/kennethreitz/requests
+.. _issue tracker: https://github.com/requests/toolbelt/issues
+
+
+History
+=======
+
+1.0.0 -- 2023-05-01
+-------------------
+
+Breaking Changes
+~~~~~~~~~~~~~~~~
+
+- Removed Google App Engine support to allow using urllib3 2.0
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Ensured the test suite no longer reaches the Internet
+
+Miscellaneous
+~~~~~~~~~~~~~
+
+- Added explicit support for Python 3.11
+
+0.10.1 -- 2022-10-25
+--------------------
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fix urllib3 warning to only emit on X509Adapter usage
+
+0.10.0 -- 2022-10-06
+--------------------
+
+New Features
+~~~~~~~~~~~~
+
+- Add support for preparing requests in BaseUrlSession
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fixing missing newline in dump utility
+
+0.9.1 -- 2019-01-29
+-------------------
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fix import of pyOpenSSL shim from urllib3 for PKCS12 adapter
+
+0.9.0 -- 2019-01-29
+-------------------
+
+New Features
+~~~~~~~~~~~~
+
+- Add X509 Adapter that can handle PKCS12
+- Add stateless solution for streaming files by MultipartEncoder from one host to another (in chunks)
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Update link to example
+- Move import of ``ABCs`` from collections into version-specific part of
+  _compat module
+- Fix backwards incompatibility in ``get_encodings_from_content``
+- Correct callback documentation for ``MultipartEncoderMonitor``
+- Fix bug when ``MultipartEncoder`` is asked to encode zero parts
+- Correct the type of non string request body dumps
+- Removed content from being stored in MultipartDecoder
+- Fix bug by enabling support for contenttype with capital letters.
+- Coerce proxy URL to bytes before dumping request
+- Avoid bailing out with exception upon empty response reason
+- Corrected Pool documentation
+- Corrected parentheses match in example usage
+- Fix "oject" to "object" in ``MultipartEncoder``
+- Fix URL for the project after the move
+- Add fix for OSX TCPKeepAliveAdapter
+
+Miscellaneous
+~~~~~~~~~~~~~
+
+- Remove py33 from testing and add Python 3.6 and nightly testing to the travis matrix.
+
+0.8.0 -- 2017-05-20
+-------------------
+
+More information about this release can be found on the `0.8.0 milestone`_.
+
+New Features
+~~~~~~~~~~~~
+
+- Add ``UserAgentBuilder`` to provide more control over generated User-Agent
+  strings.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Include ``_validate_certificate`` in the lits of picked attributes on the
+  ``AppEngineAdapter``.
+- Fix backwards incompatibility in ``get_encodings_from_content``
+
+.. _0.8.0 milestone:
+    https://github.com/requests/toolbelt/milestones/0.8.0
+
+0.7.1 -- 2017-02-13
+-------------------
+
+More information about this release can be found on the `0.7.1 milestone`_.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fixed monkey-patching for the AppEngineAdapter.
+
+- Make it easier to disable certificate verification when monkey-patching
+  AppEngine.
+
+- Handle ``multipart/form-data`` bodies without a trailing ``CRLF``.
+
+
+.. links
+.. _0.7.1 milestone:
+    https://github.com/requests/toolbelt/milestone/9
+
+0.7.0 -- 2016-07-21
+-------------------
+
+More information about this release can be found on the `0.7.0 milestone`_.
+
+New Features
+~~~~~~~~~~~~
+
+- Add ``BaseUrlSession`` to allow developers to have a session that has a
+  "Base" URL. See the documentation for more details and examples.
+
+- Split the logic of ``stream_response_to_file`` into two separate functions:
+
+  * ``get_download_file_path`` to generate the file name from the Response.
+
+  * ``stream_response_to_file`` which will use ``get_download_file_path`` if
+    necessary
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fixed the issue for people using *very* old versions of Requests where they
+  would see an ImportError from ``requests_toolbelt._compat`` when trying to
+  import ``connection``.
+
+
+.. _0.7.0 milestone:
+    https://github.com/requests/toolbelt/milestones/0.7.0
+
+0.6.2 -- 2016-05-10
+-------------------
+
+Fixed Bugs
+~~~~~~~~~~
+
+- When passing a timeout via Requests, it was not appropriately translated to
+  the timeout that the urllib3 code was expecting.
+
+0.6.1 -- 2016-05-05
+-------------------
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Remove assertion about request URLs in the AppEngineAdapter.
+
+- Prevent pip from installing requests 3.0.0 when that is released until we
+  are ready to handle it.
+
+0.6.0 -- 2016-01-27
+-------------------
+
+More information about this release can be found on the `0.6.0 milestone`_.
+
+New Features
+~~~~~~~~~~~~
+
+- Add ``AppEngineAdapter`` to support developers using Google's AppEngine
+  platform with Requests.
+
+- Add ``GuessProxyAuth`` class to support guessing between Basic and Digest
+  Authentication for proxies.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Ensure that proxies use the correct TLS version when using the
+  ``SSLAdapter``.
+
+- Fix an ``AttributeError`` when using the ``HTTPProxyDigestAuth`` class.
+
+Miscellaneous
+~~~~~~~~~~~~~
+
+- Drop testing support for Python 3.2. virtualenv and pip have stopped
+  supporting it meaning that it is harder to test for this with our CI
+  infrastructure. Moving forward we will make a best-effort attempt to
+  support 3.2 but will not test for it.
+
+
+.. _0.6.0 milestone:
+    https://github.com/requests/toolbelt/milestones/0.6.0
+
+0.5.1 -- 2015-12-16
+-------------------
+
+More information about this release can be found on the `0.5.1 milestone`_.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Now papers over the differences in requests' ``super_len`` function from
+  versions prior to 2.9.0 and versions 2.9.0 and later.
+
+
+.. _0.5.1 milestone:
+    https://github.com/requests/toolbelt/milestones/0.5.1
+
+0.5.0 -- 2015-11-24
+-------------------
+
+More information about this release can be found on the `milestone
+<https://github.com/requests/toolbelt/issues?utf8=%E2%9C%93&q=is%3Aall+milestone%3A0.5+>`_
+for 0.5.0.
+
+New Features
+~~~~~~~~~~~~
+
+- The ``tee`` submodule was added to ``requests_toolbelt.downloadutils``. It
+  allows you to iterate over the bytes of a response while also writing them
+  to a file. The ``tee.tee`` function, expects you to pass an open file
+  object, while ``tee.tee_to_file`` will use the provided file name to open
+  the file for you.
+
+- Added a new parameter to ``requests_toolbelt.utils.user_agent`` that allows
+  the user to specify additional items.
+
+- Added nested form-data helper,
+  ``requests_toolbelt.utils.formdata.urlencode``.
+
+- Added the ``ForgetfulCookieJar`` to ``requests_toolbelt.cookies``.
+
+- Added utilities for dumping the information about a request-response cycle
+  in ``requests_toolbelt.utils.dump``.
+
+- Implemented the API described in the ``requests_toolbelt.threaded`` module
+  docstring, i.e., added ``requests_toolbelt.threaded.map`` as an available
+  function.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Now papers over the API differences in versions of requests installed from
+  system packages versus versions of requests installed from PyPI.
+
+- Allow string types for ``SourceAddressAdapter``.
+
+0.4.0 -- 2015-04-03
+-------------------
+
+For more information about this release, please see `milestone 0.4.0
+<https://github.com/requests/toolbelt/issues?q=milestone%3A0.4>`_
+on the project's page.
+
+New Features
+~~~~~~~~~~~~
+
+- A naive implemenation of a thread pool is now included in the toolbelt. See
+  the docs in ``docs/threading.rst`` or on `Read The Docs
+  <https://toolbelt.readthedocs.io/>`_.
+
+- The ``StreamingIterator`` now accepts files (such as ``sys.stdin``) without
+  a specific length and will properly stream them.
+
+- The ``MultipartEncoder`` now accepts exactly the same format of fields as
+  requests' ``files`` parameter does. In other words, you can now also pass in
+  extra headers to add to a part in the body. You can also now specify a
+  custom ``Content-Type`` for a part.
+
+- An implementation of HTTP Digest Authentication for Proxies is now included.
+
+- A transport adapter that allows a user to specify a specific Certificate
+  Fingerprint is now included in the toolbelt.
+
+- A transport adapter that simplifies how users specify socket options is now
+  included.
+
+- A transport adapter that simplifies how users can specify TCP Keep-Alive
+  options is now included in the toolbelt.
+
+- Deprecated functions from ``requests.utils`` are now included and
+  maintained.
+
+- An authentication tool that allows users to specify how to authenticate to
+  several different domains at once is now included.
+
+- A function to save streamed responses to disk by analyzing the
+  ``Content-Disposition`` header is now included in the toolbelt.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- The ``MultipartEncoder`` will now allow users to upload files larger than
+  4GB on 32-bit systems.
+
+- The ``MultipartEncoder`` will now accept empty unicode strings for form
+  values.
+
+0.3.1 -- 2014-06-23
+-------------------
+
+- Fix the fact that 0.3.0 bundle did not include the ``StreamingIterator``
+
+0.3.0 -- 2014-05-21
+-------------------
+
+Bug Fixes
+~~~~~~~~~
+
+- Complete rewrite of ``MultipartEncoder`` fixes bug where bytes were lost in
+  uploads
+
+New Features
+~~~~~~~~~~~~
+
+- ``MultipartDecoder`` to accept ``multipart/form-data`` response bodies and
+  parse them into an easy to use object.
+
+- ``SourceAddressAdapter`` to allow users to choose a local address to bind
+  connections to.
+
+- ``GuessAuth`` which accepts a username and password and uses the
+  ``WWW-Authenticate`` header to determine how to authenticate against a
+  server.
+
+- ``MultipartEncoderMonitor`` wraps an instance of the ``MultipartEncoder``
+  and keeps track of how many bytes were read and will call the provided
+  callback.
+
+- ``StreamingIterator`` will wrap an iterator and stream the upload instead of
+  chunk it, provided you also provide the length of the content you wish to
+  upload.
+
+0.2.0 -- 2014-02-24
+-------------------
+
+- Add ability to tell ``MultipartEncoder`` which encoding to use. By default
+  it uses 'utf-8'.
+
+- Fix #10 - allow users to install with pip
+
+- Fix #9 - Fix ``MultipartEncoder#to_string`` so that it properly handles file
+  objects as fields
+
+0.1.2 -- 2014-01-19
+-------------------
+
+- At some point during development we broke how we handle normal file objects.
+  Thanks to @konomae this is now fixed.
+
+0.1.1 -- 2014-01-19
+-------------------
+
+- Handle ``io.BytesIO``-like objects better
+
+0.1.0 -- 2014-01-18
+-------------------
+
+- Add initial implementation of the streaming ``MultipartEncoder``
+
+- Add initial implementation of the ``user_agent`` function
+
+- Add the ``SSLAdapter``
```

### Comparing `requests-toolbelt-0.9.1/PKG-INFO` & `requests-toolbelt-1.0.0/requests_toolbelt.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,479 +1,520 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: requests-toolbelt
-Version: 0.9.1
+Version: 1.0.0
 Summary: A utility belt for advanced users of python-requests
-Home-page: https://toolbelt.readthedocs.org
+Home-page: https://toolbelt.readthedocs.io/
 Author: Ian Cordasco, Cory Benfield
 Author-email: graffatcolmingov@gmail.com
 License: Apache 2.0
-Description: The Requests Toolbelt
-        =====================
-        
-        This is just a collection of utilities for `python-requests`_, but don't 
-        really belong in ``requests`` proper. The minimum tested requests version is 
-        ``2.1.0``. In reality, the toolbelt should work with ``2.0.1`` as well, but 
-        some idiosyncracies prevent effective or sane testing on that version.
-        
-        ``pip install requests-toolbelt`` to get started!
-        
-        
-        multipart/form-data Encoder
-        ---------------------------
-        
-        The main attraction is a streaming multipart form-data object, ``MultipartEncoder``.
-        Its API looks like this:
-        
-        .. code-block:: python
-        
-            from requests_toolbelt import MultipartEncoder
-            import requests
-        
-            m = MultipartEncoder(
-                fields={'field0': 'value', 'field1': 'value',
-                        'field2': ('filename', open('file.py', 'rb'), 'text/plain')}
-                )
-        
-            r = requests.post('http://httpbin.org/post', data=m,
-                              headers={'Content-Type': m.content_type})
-        
-        
-        You can also use ``multipart/form-data`` encoding for requests that don't
-        require files:
-        
-        .. code-block:: python
-        
-            from requests_toolbelt import MultipartEncoder
-            import requests
-        
-            m = MultipartEncoder(fields={'field0': 'value', 'field1': 'value'})
-        
-            r = requests.post('http://httpbin.org/post', data=m,
-                              headers={'Content-Type': m.content_type})
-        
-        
-        Or, you can just create the string and examine the data:
-        
-        .. code-block:: python
-        
-            # Assuming `m` is one of the above
-            m.to_string()  # Always returns unicode
-        
-        
-        User-Agent constructor
-        ----------------------
-        
-        You can easily construct a requests-style ``User-Agent`` string::
-        
-            from requests_toolbelt import user_agent
-        
-            headers = {
-                'User-Agent': user_agent('my_package', '0.0.1')
-                }
-        
-            r = requests.get('https://api.github.com/users', headers=headers)
-        
-        
-        SSLAdapter
-        ----------
-        
-        The ``SSLAdapter`` was originally published on `Cory Benfield's blog`_. 
-        This adapter allows the user to choose one of the SSL protocols made available 
-        in Python's ``ssl`` module for outgoing HTTPS connections:
-        
-        .. code-block:: python
-        
-            from requests_toolbelt import SSLAdapter
-            import requests
-            import ssl
-        
-            s = requests.Session()
-            s.mount('https://', SSLAdapter(ssl.PROTOCOL_TLSv1))
-        
-        cookies/ForgetfulCookieJar
-        --------------------------
-        
-        The ``ForgetfulCookieJar`` prevents a particular requests session from storing 
-        cookies:
-        
-        .. code-block:: python
-        
-            from requests_toolbelt.cookies.forgetful import ForgetfulCookieJar
-        
-            session = requests.Session()
-            session.cookies = ForgetfulCookieJar()
-        
-        Known Issues
-        ------------
-        
-        On Python 3.3.0 and 3.3.1, the standard library's ``http`` module will fail
-        when passing an instance of the ``MultipartEncoder``. This is fixed in later
-        minor releases of Python 3.3. Please consider upgrading to a later minor
-        version or Python 3.4. *There is absolutely nothing this library can do to
-        work around that bug.*
-        
-        Contributing
-        ------------
-        
-        Please read the `suggested workflow
-        <https://toolbelt.readthedocs.org/en/latest/contributing.html>`_ for
-        contributing to this project.
-        
-        Please report any bugs on the `issue tracker`_
-        
-        .. _Cory Benfield's blog: https://lukasa.co.uk/2013/01/Choosing_SSL_Version_In_Requests/
-        .. _python-requests: https://github.com/kennethreitz/requests
-        .. _issue tracker: https://github.com/requests/toolbelt/issues
-        
-        
-        History
-        =======
-        
-        0.9.1 -- 2019-01-29
-        -------------------
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Fix import of pyOpenSSL shim from urllib3 for PKCS12 adapter
-        
-        0.9.0 -- 2019-01-29
-        -------------------
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - Add X509 Adapter that can handle PKCS12 
-        - Add stateless solution for streaming files by MultipartEncoder from one host to another (in chunks)
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Update link to example
-        - Move import of ``ABCs`` from collections into version-specific part of
-          _compat module
-        - Fix backwards incompatibility in ``get_encodings_from_content``
-        - Correct callback documentation for ``MultipartEncoderMonitor``
-        - Fix bug when ``MultipartEncoder`` is asked to encode zero parts
-        - Correct the type of non string request body dumps
-        - Removed content from being stored in MultipartDecoder
-        - Fix bug by enabling support for contenttype with capital letters. 
-        - Coerce proxy URL to bytes before dumping request
-        - Avoid bailing out with exception upon empty response reason
-        - Corrected Pool documentation
-        - Corrected parentheses match in example usage
-        - Fix "oject" to "object" in ``MultipartEncoder``
-        - Fix URL for the project after the move 
-        - Add fix for OSX TCPKeepAliveAdapter
-        
-        Miscellaneous
-        ~~~~~~~~~~~~~
-        
-        - Remove py33 from testing and add Python 3.6 and nightly testing to the travis matrix.
-        
-        0.8.0 -- 2017-05-20
-        -------------------
-        
-        More information about this release can be found on the `0.8.0 milestone`_.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - Add ``UserAgentBuilder`` to provide more control over generated User-Agent
-          strings.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Include ``_validate_certificate`` in the lits of picked attributes on the
-          ``AppEngineAdapter``.
-        - Fix backwards incompatibility in ``get_encodings_from_content``
-        
-        .. _0.8.0 milestone:
-            https://github.com/requests/toolbelt/milestones/0.8.0
-        
-        0.7.1 -- 2017-02-13
-        -------------------
-        
-        More information about this release can be found on the `0.7.1 milestone`_.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Fixed monkey-patching for the AppEngineAdapter.
-        
-        - Make it easier to disable certificate verification when monkey-patching
-          AppEngine.
-        
-        - Handle ``multipart/form-data`` bodies without a trailing ``CRLF``.
-        
-        
-        .. links
-        .. _0.7.1 milestone:
-            https://github.com/requests/toolbelt/milestone/9
-        
-        0.7.0 -- 2016-07-21
-        -------------------
-        
-        More information about this release can be found on the `0.7.0 milestone`_.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - Add ``BaseUrlSession`` to allow developers to have a session that has a
-          "Base" URL. See the documentation for more details and examples.
-        
-        - Split the logic of ``stream_response_to_file`` into two separate functions:
-        
-          * ``get_download_file_path`` to generate the file name from the Response.
-        
-          * ``stream_response_to_file`` which will use ``get_download_file_path`` if
-            necessary
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Fixed the issue for people using *very* old versions of Requests where they
-          would see an ImportError from ``requests_toolbelt._compat`` when trying to
-          import ``connection``.
-        
-        
-        .. _0.7.0 milestone:
-            https://github.com/requests/toolbelt/milestones/0.7.0
-        
-        0.6.2 -- 2016-05-10
-        -------------------
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - When passing a timeout via Requests, it was not appropriately translated to
-          the timeout that the urllib3 code was expecting.
-        
-        0.6.1 -- 2016-05-05
-        -------------------
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Remove assertion about request URLs in the AppEngineAdapter.
-        
-        - Prevent pip from installing requests 3.0.0 when that is released until we
-          are ready to handle it.
-        
-        0.6.0 -- 2016-01-27
-        -------------------
-        
-        More information about this release can be found on the `0.6.0 milestone`_.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - Add ``AppEngineAdapter`` to support developers using Google's AppEngine
-          platform with Requests.
-        
-        - Add ``GuessProxyAuth`` class to support guessing between Basic and Digest
-          Authentication for proxies.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Ensure that proxies use the correct TLS version when using the
-          ``SSLAdapter``.
-        
-        - Fix an ``AttributeError`` when using the ``HTTPProxyDigestAuth`` class.
-        
-        Miscellaneous
-        ~~~~~~~~~~~~~
-        
-        - Drop testing support for Python 3.2. virtualenv and pip have stopped
-          supporting it meaning that it is harder to test for this with our CI
-          infrastructure. Moving forward we will make a best-effort attempt to
-          support 3.2 but will not test for it.
-        
-        
-        .. _0.6.0 milestone:
-            https://github.com/requests/toolbelt/milestones/0.6.0
-        
-        0.5.1 -- 2015-12-16
-        -------------------
-        
-        More information about this release can be found on the `0.5.1 milestone`_.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Now papers over the differences in requests' ``super_len`` function from
-          versions prior to 2.9.0 and versions 2.9.0 and later.
-        
-        
-        .. _0.5.1 milestone:
-            https://github.com/requests/toolbelt/milestones/0.5.1
-        
-        0.5.0 -- 2015-11-24
-        -------------------
-        
-        More information about this release can be found on the `milestone
-        <https://github.com/requests/toolbelt/issues?utf8=%E2%9C%93&q=is%3Aall+milestone%3A0.5+>`_
-        for 0.5.0.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - The ``tee`` submodule was added to ``requests_toolbelt.downloadutils``. It
-          allows you to iterate over the bytes of a response while also writing them
-          to a file. The ``tee.tee`` function, expects you to pass an open file
-          object, while ``tee.tee_to_file`` will use the provided file name to open
-          the file for you.
-        
-        - Added a new parameter to ``requests_toolbelt.utils.user_agent`` that allows
-          the user to specify additional items.
-        
-        - Added nested form-data helper,
-          ``requests_toolbelt.utils.formdata.urlencode``.
-        
-        - Added the ``ForgetfulCookieJar`` to ``requests_toolbelt.cookies``.
-        
-        - Added utilities for dumping the information about a request-response cycle
-          in ``requests_toolbelt.utils.dump``.
-        
-        - Implemented the API described in the ``requests_toolbelt.threaded`` module
-          docstring, i.e., added ``requests_toolbelt.threaded.map`` as an available
-          function.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - Now papers over the API differences in versions of requests installed from
-          system packages versus versions of requests installed from PyPI.
-        
-        - Allow string types for ``SourceAddressAdapter``.
-        
-        0.4.0 -- 2015-04-03
-        -------------------
-        
-        For more information about this release, please see `milestone 0.4.0
-        <https://github.com/requests/toolbelt/issues?q=milestone%3A0.4>`_
-        on the project's page.
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - A naive implemenation of a thread pool is now included in the toolbelt. See
-          the docs in ``docs/threading.rst`` or on `Read The Docs
-          <https://toolbelt.readthedocs.org>`_.
-        
-        - The ``StreamingIterator`` now accepts files (such as ``sys.stdin``) without
-          a specific length and will properly stream them.
-        
-        - The ``MultipartEncoder`` now accepts exactly the same format of fields as
-          requests' ``files`` parameter does. In other words, you can now also pass in
-          extra headers to add to a part in the body. You can also now specify a
-          custom ``Content-Type`` for a part.
-        
-        - An implementation of HTTP Digest Authentication for Proxies is now included.
-        
-        - A transport adapter that allows a user to specify a specific Certificate
-          Fingerprint is now included in the toolbelt.
-        
-        - A transport adapter that simplifies how users specify socket options is now
-          included.
-        
-        - A transport adapter that simplifies how users can specify TCP Keep-Alive
-          options is now included in the toolbelt.
-        
-        - Deprecated functions from ``requests.utils`` are now included and
-          maintained.
-        
-        - An authentication tool that allows users to specify how to authenticate to
-          several different domains at once is now included.
-        
-        - A function to save streamed responses to disk by analyzing the
-          ``Content-Disposition`` header is now included in the toolbelt.
-        
-        Fixed Bugs
-        ~~~~~~~~~~
-        
-        - The ``MultipartEncoder`` will now allow users to upload files larger than
-          4GB on 32-bit systems.
-        
-        - The ``MultipartEncoder`` will now accept empty unicode strings for form
-          values.
-        
-        0.3.1 -- 2014-06-23
-        -------------------
-        
-        - Fix the fact that 0.3.0 bundle did not include the ``StreamingIterator``
-        
-        0.3.0 -- 2014-05-21
-        -------------------
-        
-        Bug Fixes
-        ~~~~~~~~~
-        
-        - Complete rewrite of ``MultipartEncoder`` fixes bug where bytes were lost in
-          uploads
-        
-        New Features
-        ~~~~~~~~~~~~
-        
-        - ``MultipartDecoder`` to accept ``multipart/form-data`` response bodies and
-          parse them into an easy to use object.
-        
-        - ``SourceAddressAdapter`` to allow users to choose a local address to bind
-          connections to.
-        
-        - ``GuessAuth`` which accepts a username and password and uses the
-          ``WWW-Authenticate`` header to determine how to authenticate against a
-          server.
-        
-        - ``MultipartEncoderMonitor`` wraps an instance of the ``MultipartEncoder``
-          and keeps track of how many bytes were read and will call the provided
-          callback.
-        
-        - ``StreamingIterator`` will wrap an iterator and stream the upload instead of
-          chunk it, provided you also provide the length of the content you wish to
-          upload.
-        
-        0.2.0 -- 2014-02-24
-        -------------------
-        
-        - Add ability to tell ``MultipartEncoder`` which encoding to use. By default
-          it uses 'utf-8'.
-        
-        - Fix #10 - allow users to install with pip
-        
-        - Fix #9 - Fix ``MultipartEncoder#to_string`` so that it properly handles file
-          objects as fields
-        
-        0.1.2 -- 2014-01-19
-        -------------------
-        
-        - At some point during development we broke how we handle normal file objects.
-          Thanks to @konomae this is now fixed.
-        
-        0.1.1 -- 2014-01-19
-        -------------------
-        
-        - Handle ``io.BytesIO``-like objects better
-        
-        0.1.0 -- 2014-01-18
-        -------------------
-        
-        - Add initial implementation of the streaming ``MultipartEncoder``
-        
-        - Add initial implementation of the ``user_agent`` function
-        
-        - Add the ``SSLAdapter``
-        
-Platform: UNKNOWN
+Project-URL: Changelog, https://github.com/requests/toolbelt/blob/master/HISTORY.rst
+Project-URL: Source, https://github.com/requests/toolbelt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+License-File: AUTHORS.rst
+
+The Requests Toolbelt
+=====================
+
+This is just a collection of utilities for `python-requests`_, but don't
+really belong in ``requests`` proper. The minimum tested requests version is
+``2.1.0``. In reality, the toolbelt should work with ``2.0.1`` as well, but
+some idiosyncracies prevent effective or sane testing on that version.
+
+``pip install requests-toolbelt`` to get started!
+
+
+multipart/form-data Encoder
+---------------------------
+
+The main attraction is a streaming multipart form-data object, ``MultipartEncoder``.
+Its API looks like this:
+
+.. code-block:: python
+
+    from requests_toolbelt import MultipartEncoder
+    import requests
+
+    m = MultipartEncoder(
+        fields={'field0': 'value', 'field1': 'value',
+                'field2': ('filename', open('file.py', 'rb'), 'text/plain')}
+        )
+
+    r = requests.post('http://httpbin.org/post', data=m,
+                      headers={'Content-Type': m.content_type})
+
+
+You can also use ``multipart/form-data`` encoding for requests that don't
+require files:
+
+.. code-block:: python
+
+    from requests_toolbelt import MultipartEncoder
+    import requests
+
+    m = MultipartEncoder(fields={'field0': 'value', 'field1': 'value'})
+
+    r = requests.post('http://httpbin.org/post', data=m,
+                      headers={'Content-Type': m.content_type})
+
+
+Or, you can just create the string and examine the data:
+
+.. code-block:: python
+
+    # Assuming `m` is one of the above
+    m.to_string()  # Always returns unicode
+
+
+User-Agent constructor
+----------------------
+
+You can easily construct a requests-style ``User-Agent`` string::
+
+    from requests_toolbelt import user_agent
+
+    headers = {
+        'User-Agent': user_agent('my_package', '0.0.1')
+        }
+
+    r = requests.get('https://api.github.com/users', headers=headers)
+
+
+SSLAdapter
+----------
+
+The ``SSLAdapter`` was originally published on `Cory Benfield's blog`_.
+This adapter allows the user to choose one of the SSL protocols made available
+in Python's ``ssl`` module for outgoing HTTPS connections:
+
+.. code-block:: python
+
+    from requests_toolbelt import SSLAdapter
+    import requests
+    import ssl
+
+    s = requests.Session()
+    s.mount('https://', SSLAdapter(ssl.PROTOCOL_TLSv1))
+
+cookies/ForgetfulCookieJar
+--------------------------
+
+The ``ForgetfulCookieJar`` prevents a particular requests session from storing
+cookies:
+
+.. code-block:: python
+
+    from requests_toolbelt.cookies.forgetful import ForgetfulCookieJar
+
+    session = requests.Session()
+    session.cookies = ForgetfulCookieJar()
+
+Contributing
+------------
+
+Please read the `suggested workflow
+<https://toolbelt.readthedocs.io/en/latest/contributing.html>`_ for
+contributing to this project.
+
+Please report any bugs on the `issue tracker`_
+
+.. _Cory Benfield's blog: https://lukasa.co.uk/2013/01/Choosing_SSL_Version_In_Requests/
+.. _python-requests: https://github.com/kennethreitz/requests
+.. _issue tracker: https://github.com/requests/toolbelt/issues
+
+
+History
+=======
+
+1.0.0 -- 2023-05-01
+-------------------
+
+Breaking Changes
+~~~~~~~~~~~~~~~~
+
+- Removed Google App Engine support to allow using urllib3 2.0
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Ensured the test suite no longer reaches the Internet
+
+Miscellaneous
+~~~~~~~~~~~~~
+
+- Added explicit support for Python 3.11
+
+0.10.1 -- 2022-10-25
+--------------------
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fix urllib3 warning to only emit on X509Adapter usage
+
+0.10.0 -- 2022-10-06
+--------------------
+
+New Features
+~~~~~~~~~~~~
+
+- Add support for preparing requests in BaseUrlSession
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fixing missing newline in dump utility
+
+0.9.1 -- 2019-01-29
+-------------------
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fix import of pyOpenSSL shim from urllib3 for PKCS12 adapter
+
+0.9.0 -- 2019-01-29
+-------------------
+
+New Features
+~~~~~~~~~~~~
+
+- Add X509 Adapter that can handle PKCS12
+- Add stateless solution for streaming files by MultipartEncoder from one host to another (in chunks)
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Update link to example
+- Move import of ``ABCs`` from collections into version-specific part of
+  _compat module
+- Fix backwards incompatibility in ``get_encodings_from_content``
+- Correct callback documentation for ``MultipartEncoderMonitor``
+- Fix bug when ``MultipartEncoder`` is asked to encode zero parts
+- Correct the type of non string request body dumps
+- Removed content from being stored in MultipartDecoder
+- Fix bug by enabling support for contenttype with capital letters.
+- Coerce proxy URL to bytes before dumping request
+- Avoid bailing out with exception upon empty response reason
+- Corrected Pool documentation
+- Corrected parentheses match in example usage
+- Fix "oject" to "object" in ``MultipartEncoder``
+- Fix URL for the project after the move
+- Add fix for OSX TCPKeepAliveAdapter
+
+Miscellaneous
+~~~~~~~~~~~~~
+
+- Remove py33 from testing and add Python 3.6 and nightly testing to the travis matrix.
+
+0.8.0 -- 2017-05-20
+-------------------
+
+More information about this release can be found on the `0.8.0 milestone`_.
+
+New Features
+~~~~~~~~~~~~
+
+- Add ``UserAgentBuilder`` to provide more control over generated User-Agent
+  strings.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Include ``_validate_certificate`` in the lits of picked attributes on the
+  ``AppEngineAdapter``.
+- Fix backwards incompatibility in ``get_encodings_from_content``
+
+.. _0.8.0 milestone:
+    https://github.com/requests/toolbelt/milestones/0.8.0
+
+0.7.1 -- 2017-02-13
+-------------------
+
+More information about this release can be found on the `0.7.1 milestone`_.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fixed monkey-patching for the AppEngineAdapter.
+
+- Make it easier to disable certificate verification when monkey-patching
+  AppEngine.
+
+- Handle ``multipart/form-data`` bodies without a trailing ``CRLF``.
+
+
+.. links
+.. _0.7.1 milestone:
+    https://github.com/requests/toolbelt/milestone/9
+
+0.7.0 -- 2016-07-21
+-------------------
+
+More information about this release can be found on the `0.7.0 milestone`_.
+
+New Features
+~~~~~~~~~~~~
+
+- Add ``BaseUrlSession`` to allow developers to have a session that has a
+  "Base" URL. See the documentation for more details and examples.
+
+- Split the logic of ``stream_response_to_file`` into two separate functions:
+
+  * ``get_download_file_path`` to generate the file name from the Response.
+
+  * ``stream_response_to_file`` which will use ``get_download_file_path`` if
+    necessary
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Fixed the issue for people using *very* old versions of Requests where they
+  would see an ImportError from ``requests_toolbelt._compat`` when trying to
+  import ``connection``.
+
+
+.. _0.7.0 milestone:
+    https://github.com/requests/toolbelt/milestones/0.7.0
+
+0.6.2 -- 2016-05-10
+-------------------
+
+Fixed Bugs
+~~~~~~~~~~
+
+- When passing a timeout via Requests, it was not appropriately translated to
+  the timeout that the urllib3 code was expecting.
+
+0.6.1 -- 2016-05-05
+-------------------
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Remove assertion about request URLs in the AppEngineAdapter.
+
+- Prevent pip from installing requests 3.0.0 when that is released until we
+  are ready to handle it.
+
+0.6.0 -- 2016-01-27
+-------------------
+
+More information about this release can be found on the `0.6.0 milestone`_.
+
+New Features
+~~~~~~~~~~~~
+
+- Add ``AppEngineAdapter`` to support developers using Google's AppEngine
+  platform with Requests.
+
+- Add ``GuessProxyAuth`` class to support guessing between Basic and Digest
+  Authentication for proxies.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Ensure that proxies use the correct TLS version when using the
+  ``SSLAdapter``.
+
+- Fix an ``AttributeError`` when using the ``HTTPProxyDigestAuth`` class.
+
+Miscellaneous
+~~~~~~~~~~~~~
+
+- Drop testing support for Python 3.2. virtualenv and pip have stopped
+  supporting it meaning that it is harder to test for this with our CI
+  infrastructure. Moving forward we will make a best-effort attempt to
+  support 3.2 but will not test for it.
+
+
+.. _0.6.0 milestone:
+    https://github.com/requests/toolbelt/milestones/0.6.0
+
+0.5.1 -- 2015-12-16
+-------------------
+
+More information about this release can be found on the `0.5.1 milestone`_.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Now papers over the differences in requests' ``super_len`` function from
+  versions prior to 2.9.0 and versions 2.9.0 and later.
+
+
+.. _0.5.1 milestone:
+    https://github.com/requests/toolbelt/milestones/0.5.1
+
+0.5.0 -- 2015-11-24
+-------------------
+
+More information about this release can be found on the `milestone
+<https://github.com/requests/toolbelt/issues?utf8=%E2%9C%93&q=is%3Aall+milestone%3A0.5+>`_
+for 0.5.0.
+
+New Features
+~~~~~~~~~~~~
+
+- The ``tee`` submodule was added to ``requests_toolbelt.downloadutils``. It
+  allows you to iterate over the bytes of a response while also writing them
+  to a file. The ``tee.tee`` function, expects you to pass an open file
+  object, while ``tee.tee_to_file`` will use the provided file name to open
+  the file for you.
+
+- Added a new parameter to ``requests_toolbelt.utils.user_agent`` that allows
+  the user to specify additional items.
+
+- Added nested form-data helper,
+  ``requests_toolbelt.utils.formdata.urlencode``.
+
+- Added the ``ForgetfulCookieJar`` to ``requests_toolbelt.cookies``.
+
+- Added utilities for dumping the information about a request-response cycle
+  in ``requests_toolbelt.utils.dump``.
+
+- Implemented the API described in the ``requests_toolbelt.threaded`` module
+  docstring, i.e., added ``requests_toolbelt.threaded.map`` as an available
+  function.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- Now papers over the API differences in versions of requests installed from
+  system packages versus versions of requests installed from PyPI.
+
+- Allow string types for ``SourceAddressAdapter``.
+
+0.4.0 -- 2015-04-03
+-------------------
+
+For more information about this release, please see `milestone 0.4.0
+<https://github.com/requests/toolbelt/issues?q=milestone%3A0.4>`_
+on the project's page.
+
+New Features
+~~~~~~~~~~~~
+
+- A naive implemenation of a thread pool is now included in the toolbelt. See
+  the docs in ``docs/threading.rst`` or on `Read The Docs
+  <https://toolbelt.readthedocs.io/>`_.
+
+- The ``StreamingIterator`` now accepts files (such as ``sys.stdin``) without
+  a specific length and will properly stream them.
+
+- The ``MultipartEncoder`` now accepts exactly the same format of fields as
+  requests' ``files`` parameter does. In other words, you can now also pass in
+  extra headers to add to a part in the body. You can also now specify a
+  custom ``Content-Type`` for a part.
+
+- An implementation of HTTP Digest Authentication for Proxies is now included.
+
+- A transport adapter that allows a user to specify a specific Certificate
+  Fingerprint is now included in the toolbelt.
+
+- A transport adapter that simplifies how users specify socket options is now
+  included.
+
+- A transport adapter that simplifies how users can specify TCP Keep-Alive
+  options is now included in the toolbelt.
+
+- Deprecated functions from ``requests.utils`` are now included and
+  maintained.
+
+- An authentication tool that allows users to specify how to authenticate to
+  several different domains at once is now included.
+
+- A function to save streamed responses to disk by analyzing the
+  ``Content-Disposition`` header is now included in the toolbelt.
+
+Fixed Bugs
+~~~~~~~~~~
+
+- The ``MultipartEncoder`` will now allow users to upload files larger than
+  4GB on 32-bit systems.
+
+- The ``MultipartEncoder`` will now accept empty unicode strings for form
+  values.
+
+0.3.1 -- 2014-06-23
+-------------------
+
+- Fix the fact that 0.3.0 bundle did not include the ``StreamingIterator``
+
+0.3.0 -- 2014-05-21
+-------------------
+
+Bug Fixes
+~~~~~~~~~
+
+- Complete rewrite of ``MultipartEncoder`` fixes bug where bytes were lost in
+  uploads
+
+New Features
+~~~~~~~~~~~~
+
+- ``MultipartDecoder`` to accept ``multipart/form-data`` response bodies and
+  parse them into an easy to use object.
+
+- ``SourceAddressAdapter`` to allow users to choose a local address to bind
+  connections to.
+
+- ``GuessAuth`` which accepts a username and password and uses the
+  ``WWW-Authenticate`` header to determine how to authenticate against a
+  server.
+
+- ``MultipartEncoderMonitor`` wraps an instance of the ``MultipartEncoder``
+  and keeps track of how many bytes were read and will call the provided
+  callback.
+
+- ``StreamingIterator`` will wrap an iterator and stream the upload instead of
+  chunk it, provided you also provide the length of the content you wish to
+  upload.
+
+0.2.0 -- 2014-02-24
+-------------------
+
+- Add ability to tell ``MultipartEncoder`` which encoding to use. By default
+  it uses 'utf-8'.
+
+- Fix #10 - allow users to install with pip
+
+- Fix #9 - Fix ``MultipartEncoder#to_string`` so that it properly handles file
+  objects as fields
+
+0.1.2 -- 2014-01-19
+-------------------
+
+- At some point during development we broke how we handle normal file objects.
+  Thanks to @konomae this is now fixed.
+
+0.1.1 -- 2014-01-19
+-------------------
+
+- Handle ``io.BytesIO``-like objects better
+
+0.1.0 -- 2014-01-18
+-------------------
+
+- Add initial implementation of the streaming ``MultipartEncoder``
+
+- Add initial implementation of the ``user_agent`` function
+
+- Add the ``SSLAdapter``
```

### Comparing `requests-toolbelt-0.9.1/AUTHORS.rst` & `requests-toolbelt-1.0.0/AUTHORS.rst`

 * *Files 16% similar despite different names*

```diff
@@ -46,8 +46,12 @@
 
 - Yorgos Pagles <yorgos@pagles.org>
 
 - Thomas Hauk <thauk@copperleaf.com>
 
 - Achim Herwig <python@wodca.de>
 
-- Ryan Ashley <rashley-iqt>
+- Ryan Ashley <rashley-iqt>
+
+- Sam Bull (@greatestape)
+
+- Florence Blanc-Renaud <flo@redhat.com> (@flo-renaud)
```

### Comparing `requests-toolbelt-0.9.1/docs/dumputils.rst` & `requests-toolbelt-1.0.0/docs/dumputils.rst`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/docs/conf.py` & `requests-toolbelt-1.0.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,8 +264,8 @@
 #texinfo_show_urls = 'footnote'
 
 # If true, do not generate a @detailmenu in the "Top" node's menu.
 #texinfo_no_detailmenu = False
 
 
 # Example configuration for intersphinx: refer to the Python standard library.
-intersphinx_mapping = {'http://docs.python.org/': None}
+intersphinx_mapping = {'https://docs.python.org/': None}
```

### Comparing `requests-toolbelt-0.9.1/docs/threading.rst` & `requests-toolbelt-1.0.0/docs/threading.rst`

 * *Files 10% similar despite different names*

```diff
@@ -40,22 +40,22 @@
 
     jobs = queue.Queue()
     urls = [
         # My list of URLs to get
     ]
 
     for url in urls:
-        queue.put({'method': 'GET', 'url': url})
+        jobs.put({'method': 'GET', 'url': url})
 
-    p = pool.Pool(job_queue=q)
+    p = pool.Pool(job_queue=jobs)
     p.join_all()
 
     for response in p.responses():
-        print('GET {0}. Returned {1}.'.format(response.request_kwargs['url'],
-                                              response.status_code))
+        print('GET {}. Returned {}.'.format(response.request_kwargs['url'],
+                                            response.status_code))
 
 This is clearly a bit underwhelming. This is why there's a short-cut class
 method to create a :class:`~requests_toolbelt.threaded.pool.Pool` from a list
 of URLs.
 
 .. code-block:: python
 
@@ -65,16 +65,16 @@
         # My list of URLs to get
     ]
 
     p = pool.Pool.from_urls(urls)
     p.join_all()
 
     for response in p.responses():
-        print('GET {0}. Returned {1}.'.format(response.request_kwargs['url'],
-                                              response.status_code))
+        print('GET {}. Returned {}.'.format(response.request_kwargs['url'],
+                                            response.status_code))
 
 If one of the URLs in your list throws an exception, it will be accessible
 from the :meth:`~Pool.exceptions` generator.
 
 .. code-block:: python
 
     from requests_toolbelt.threaded import pool
@@ -83,16 +83,16 @@
         # My list of URLs to get
     ]
 
     p = pool.Pool.from_urls(urls)
     p.join_all()
 
     for exc in p.exceptions():
-        print('GET {0}. Raised {1}.'.format(exc.request_kwargs['url'],
-                                            exc.message))
+        print('GET {}. Raised {}.'.format(exc.request_kwargs['url'],
+                                          exc.message))
 
 If instead, you want to retry the exceptions that have been raised you can do
 the following:
 
 .. code-block:: python
 
     from requests_toolbelt.threaded import pool
```

### Comparing `requests-toolbelt-0.9.1/docs/sessions.rst` & `requests-toolbelt-1.0.0/docs/sessions.rst`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/docs/contributing.rst` & `requests-toolbelt-1.0.0/docs/contributing.rst`

 * *Files 2% similar despite different names*

```diff
@@ -153,9 +153,9 @@
 
 .. [#] If each commit has the same message, the reviewer may ask you to
        squash your commits or may squash them for you and perform a manual
        merge.
 
 .. _GitHub: https://github.com/requests/toolbelt
 .. _GitLab: https://gitlab.com/sigmavirus24/toolbelt
-.. _tox: https://tox.readthedocs.org/en/latest/
-.. _pytest: http://pytest.org/latest/
+.. _tox: https://tox.readthedocs.io/
+.. _pytest: https://docs.pytest.org/
```

### Comparing `requests-toolbelt-0.9.1/docs/adapters.rst` & `requests-toolbelt-1.0.0/docs/adapters.rst`

 * *Files 26% similar despite different names*

```diff
@@ -3,85 +3,28 @@
 Transport Adapters
 ==================
 
 The toolbelt comes with several different transport adapters for you to use
 with requests. The transport adapters are all kept in
 :mod:`requests_toolbelt.adapters` and include
 
-- :class:`requests_toolbelt.adapters.appengine.AppEngineAdapter`
-
 - :class:`requests_toolbelt.adapters.fingerprint.FingerprintAdapter`
 
 - :class:`requests_toolbelt.adapters.socket_options.SocketOptionsAdapter`
 
 - :class:`requests_toolbelt.adapters.socket_options.TCPKeepAliveAdapter`
 
 - :class:`requests_toolbelt.adapters.source.SourceAddressAdapter`
 
 - :class:`requests_toolbelt.adapters.ssl.SSLAdapter`
 
 - :class:`requests_toolbelt.adapters.host_header_ssl.HostHeaderSSLAdapter`
 
 - :class:`requests_toolbelt.adapters.x509.X509Adapter`
 
-AppEngineAdapter
-----------------
-
-.. versionadded:: 0.6.0
-
-As of version 2.10.0, Requests will be capable of supporting Google's App
-Engine platform. In order to use Requests on GAE, however, you will need a
-custom adapter found here as
-:class:`~requests_toolbelt.adapters.appengine.AppEngineAdapter`. There are two
-ways to take advantage of this support at the moment:
-
-#. Using the :class:`~requests_toolbelt.adapters.appengine.AppEngineAdapter`
-   like every other adapter, e.g.,
-
-   .. code-block:: python
-
-       import requests
-       from requests_toolbelt.adapters import appengine
-
-       s = requests.Session()
-       s.mount('http://', appengine.AppEngineAdapter())
-       s.mount('https://', appengine.AppEngineAdapter())
-
-#. By monkey-patching requests to always use the provided adapter:
-
-   .. code-block:: python
-
-       import requests
-       from requests_toolbelt.adapters import appengine
-
-       appengine.monkeypatch()
-
-.. _insecure_appengine:
-
-If you should need to disable certificate validation when monkeypatching (to
-force third-party libraries that use Requests to not validate certificates, if
-they do not provide API surface to do so, for example), you can disable it:
-
-   .. code-block:: python
-
-       from requests_toolbelt.adapters import appengine
-       appengine.monkeypatch(validate_certificate=False)
-
-   .. warning::
-
-       If ``validate_certificate`` is ``False``, the monkeypatched adapter
-       will *not* validate certificates. This effectively sets the
-       ``validate_certificate`` argument to urlfetch.Fetch() to ``False``. You
-       should avoid using this wherever possible. Details can be found in the
-       `documentation for urlfetch.Fetch()`_.
-
-       .. _documentation for urlfetch.Fetch(): https://cloud.google.com/appengine/docs/python/refdocs/google.appengine.api.urlfetch
-
-.. autoclass:: requests_toolbelt.adapters.appengine.AppEngineAdapter
-
 FingerprintAdapter
 ------------------
 
 .. versionadded:: 0.4.0
 
 By default, requests will validate a server's certificate to ensure a
 connection is secure. In addition to this, the user can provide a fingerprint
@@ -244,17 +187,17 @@
 ``http://`` request.
 
 .. autoclass:: requests_toolbelt.adapters.socket_options.TCPKeepAliveAdapter
 
 X509Adapter
 -----------
 
-Requests supports SSL Verification using a certificate in .pem format by default. 
+Requests supports SSL Verification using a certificate in .pem format by default.
 In some cases it is necessary to pass a full cert chain as part of a request or it
-is deemed too great a risk to decrypt the certificate into a .pem file.  
+is deemed too great a risk to decrypt the certificate into a .pem file.
 
 For such use cases we have created
 :class:`~requests_toolbelt.adapters.x509.X509Adapter`.
 Example usage:
 
 .. code-block:: python
 
@@ -262,8 +205,7 @@
       from requests_toolbelt.adapters.x509 import X509Adapter
       s = requests.Session()
       a = X509Adapter(max_retries=3,
                       cert_bytes=b'...', pk_bytes=b'...', encoding='...')
       s.mount('https://', a)
 
 .. autoclass:: requests_toolbelt.adapters.x509.X509Adapter
-
```

### Comparing `requests-toolbelt-0.9.1/docs/user-agent.rst` & `requests-toolbelt-1.0.0/docs/user-agent.rst`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/docs/Makefile` & `requests-toolbelt-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/docs/index.rst` & `requests-toolbelt-1.0.0/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,7 @@
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
-
```

### Comparing `requests-toolbelt-0.9.1/docs/uploading-data.rst` & `requests-toolbelt-1.0.0/docs/uploading-data.rst`

 * *Files identical despite different names*

### Comparing `requests-toolbelt-0.9.1/docs/authentication.rst` & `requests-toolbelt-1.0.0/docs/authentication.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Authentication
 ==============
 
 requests supports Basic Authentication and HTTP Digest Authentication by
 default. There are also a number of third-party libraries for authentication
 with:
 
-- `OAuth <https://requests-oauthlib.readthedocs.org/en/latest/>`_
+- `OAuth <https://requests-oauthlib.readthedocs.io/>`_
 
 - `NTLM <https://github.com/requests/requests-ntlm>`_
 
 - `Kerberos <https://github.com/requests/requests-kerberos>`_
 
 The :mod:`requests_toolbelt.auth` provides extra authentication features in
 addition to those. It provides the following authentication classes:
@@ -129,14 +129,14 @@
     from requests_toolbelt.auth.http_proxy_digest import HTTPProxyDigestAuth
 
 
     proxies = {
         "http": "http://PROXYSERVER:PROXYPORT",
         "https": "https://PROXYSERVER:PROXYPORT",
     }
-    url = "https://toolbelt.readthedocs.org/"
+    url = "https://toolbelt.readthedocs.io/"
     auth = HTTPProxyDigestAuth("USERNAME", "PASSWORD")
     requests.get(url, proxies=proxies, auth=auth)
 
 Program would raise error if the username or password is rejected by the proxy.
 
 .. autoclass:: requests_toolbelt.auth.http_proxy_digest.HTTPProxyDigestAuth
```

### Comparing `requests-toolbelt-0.9.1/docs/make.bat` & `requests-toolbelt-1.0.0/docs/make.bat`

 * *Files identical despite different names*

