# Comparing `tmp/bbot-1.0.5.1656rc0.tar.gz` & `tmp/bbot-1.0.5.1660rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbot-1.0.5.1656rc0.tar", max compression
+gzip compressed data, was "bbot-1.0.5.1660rc0.tar", max compression
```

## Comparing `bbot-1.0.5.1656rc0.tar` & `bbot-1.0.5.1660rc0.tar`

### file list

```diff
@@ -1,182 +1,182 @@
--rw-r--r--   0        0        0    32473 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/LICENSE
--rw-r--r--   0        0        0    51011 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/README.md
--rw-r--r--   0        0        0      211 2023-04-26 15:27:28.747710 bbot-1.0.5.1656rc0/bbot/__init__.py
--rw-r--r--   0        0        0       25 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/agent/__init__.py
--rw-r--r--   0        0        0     6536 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/agent/agent.py
--rw-r--r--   0        0        0      376 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/agent/messages.py
--rwxr-xr-x   0        0        0    13693 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/cli.py
--rw-r--r--   0        0        0       93 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/__init__.py
--rw-r--r--   0        0        0     3171 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/configurator/__init__.py
--rw-r--r--   0        0        0     8920 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/configurator/args.py
--rw-r--r--   0        0        0     4261 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/configurator/environ.py
--rw-r--r--   0        0        0     1170 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/configurator/files.py
--rw-r--r--   0        0        0      632 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/errors.py
--rw-r--r--   0        0        0      104 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/event/__init__.py
--rw-r--r--   0        0        0    30371 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/event/base.py
--rw-r--r--   0        0        0     1498 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/event/helpers.py
--rw-r--r--   0        0        0       61 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/__init__.py
--rw-r--r--   0        0        0     3644 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/cache.py
--rw-r--r--   0        0        0     1256 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/__init__.py
--rw-r--r--   0        0        0      565 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/aws.py
--rw-r--r--   0        0        0      716 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/azure.py
--rw-r--r--   0        0        0     2875 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/base.py
--rw-r--r--   0        0        0      297 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/digitalocean.py
--rw-r--r--   0        0        0      271 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/firebase.py
--rw-r--r--   0        0        0      352 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/gcp.py
--rw-r--r--   0        0        0     6940 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/command.py
--rw-r--r--   0        0        0       37 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/depsinstaller/__init__.py
--rw-r--r--   0        0        0    13841 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/depsinstaller/installer.py
--rw-r--r--   0        0        0       87 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
--rw-r--r--   0        0        0     8540 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/diff.py
--rw-r--r--   0        0        0    29454 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/dns.py
--rw-r--r--   0        0        0     4286 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/helper.py
--rw-r--r--   0        0        0     5435 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/interactsh.py
--rw-r--r--   0        0        0     1414 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/logger.py
--rw-r--r--   0        0        0    29037 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/misc.py
--rw-r--r--   0        0        0    14848 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/modules.py
--rw-r--r--   0        0        0     9574 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/names_generator.py
--rw-r--r--   0        0        0     2578 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/ntlm.py
--rw-r--r--   0        0        0      795 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/punycode.py
--rw-r--r--   0        0        0     2919 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/queueing.py
--rw-r--r--   0        0        0     1890 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/regexes.py
--rw-r--r--   0        0        0     8474 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/threadpool.py
--rw-r--r--   0        0        0     3987 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/url.py
--rw-r--r--   0        0        0     3193 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/validators.py
--rw-r--r--   0        0        0     9324 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/web.py
--rw-r--r--   0        0        0    10967 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/helpers/wordcloud.py
--rw-r--r--   0        0        0       99 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/logger/__init__.py
--rw-r--r--   0        0        0     7859 2023-04-26 15:26:56.495322 bbot-1.0.5.1656rc0/bbot/core/logger/logger.py
--rw-r--r--   0        0        0     2091 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/db/neo4j.py
--rw-r--r--   0        0        0     3731 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/defaults.yml
--rw-r--r--   0        0        0      396 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/__init__.py
--rw-r--r--   0        0        0     1371 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/anubisdb.py
--rw-r--r--   0        0        0     3461 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/azure_tenant.py
--rw-r--r--   0        0        0     2350 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/badsecrets.py
--rw-r--r--   0        0        0    25359 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/base.py
--rw-r--r--   0        0        0     2197 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/bevigil.py
--rw-r--r--   0        0        0     1225 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/binaryedge.py
--rw-r--r--   0        0        0     5502 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/bucket_aws.py
--rw-r--r--   0        0        0     1065 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/bucket_azure.py
--rw-r--r--   0        0        0      847 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/bucket_digitalocean.py
--rw-r--r--   0        0        0     1167 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/bucket_firebase.py
--rw-r--r--   0        0        0     2169 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/bucket_gcp.py
--rw-r--r--   0        0        0     4550 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/builtwith.py
--rw-r--r--   0        0        0     5107 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/bypass403.py
--rw-r--r--   0        0        0     1116 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/c99.py
--rw-r--r--   0        0        0     5432 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/censys.py
--rw-r--r--   0        0        0      732 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/certspotter.py
--rw-r--r--   0        0        0     5001 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/crobat.py
--rw-r--r--   0        0        0     1160 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/crt.py
--rw-r--r--   0        0        0    13578 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/deadly/ffuf.py
--rw-r--r--   0        0        0    15617 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/deadly/nuclei.py
--rw-r--r--   0        0        0     5763 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/deadly/vhost.py
--rw-r--r--   0        0        0     2516 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/dnscommonsrv.py
--rw-r--r--   0        0        0     2954 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/dnsdumpster.py
--rw-r--r--   0        0        0     2862 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/dnszonetransfer.py
--rw-r--r--   0        0        0      866 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/emailformat.py
--rw-r--r--   0        0        0    11117 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/ffuf_shortnames.py
--rw-r--r--   0        0        0     2164 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/fingerprintx.py
--rw-r--r--   0        0        0     1093 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/fullhunt.py
--rw-r--r--   0        0        0     7290 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/generic_ssrf.py
--rw-r--r--   0        0        0     2723 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/github.py
--rw-r--r--   0        0        0    10060 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/gowitness.py
--rw-r--r--   0        0        0      658 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/hackertarget.py
--rw-r--r--   0        0        0     7395 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/host_header.py
--rw-r--r--   0        0        0     5546 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/httpx.py
--rw-r--r--   0        0        0     7748 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/hunt.py
--rw-r--r--   0        0        0     1944 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/hunterio.py
--rw-r--r--   0        0        0     9438 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/iis_shortnames.py
--rw-r--r--   0        0        0        0 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/internal/__init__.py
--rw-r--r--   0        0        0      311 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/internal/aggregate.py
--rw-r--r--   0        0        0      578 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/internal/base.py
--rw-r--r--   0        0        0    16263 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/internal/excavate.py
--rw-r--r--   0        0        0     4481 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/internal/speculate.py
--rw-r--r--   0        0        0     1274 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/ipneighbor.py
--rw-r--r--   0        0        0     2037 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/ipstack.py
--rw-r--r--   0        0        0      707 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/leakix.py
--rw-r--r--   0        0        0    11237 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/masscan.py
--rw-r--r--   0        0        0    13620 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/massdns.py
--rw-r--r--   0        0        0     4245 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/naabu.py
--rw-r--r--   0        0        0     4867 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/ntlm.py
--rw-r--r--   0        0        0      728 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/otx.py
--rw-r--r--   0        0        0        0 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/__init__.py
--rw-r--r--   0        0        0     9307 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/asset_inventory.py
--rw-r--r--   0        0        0     1379 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/base.py
--rw-r--r--   0        0        0     2546 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/csv.py
--rw-r--r--   0        0        0     1809 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/http.py
--rw-r--r--   0        0        0     1787 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/human.py
--rw-r--r--   0        0        0     1007 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/json.py
--rw-r--r--   0        0        0     1255 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/neo4j.py
--rw-r--r--   0        0        0      204 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/python.py
--rw-r--r--   0        0        0     3609 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/web_report.py
--rw-r--r--   0        0        0     1747 2023-04-26 15:26:56.499322 bbot-1.0.5.1656rc0/bbot/modules/output/websocket.py
--rw-r--r--   0        0        0     1532 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/paramminer_cookies.py
--rw-r--r--   0        0        0     1620 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/paramminer_getparams.py
--rw-r--r--   0        0        0     5360 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/paramminer_headers.py
--rw-r--r--   0        0        0     1533 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/passivetotal.py
--rw-r--r--   0        0        0     1310 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/pgp.py
--rw-r--r--   0        0        0      746 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/rapiddns.py
--rw-r--r--   0        0        0     1606 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/report/affiliates.py
--rw-r--r--   0        0        0     8304 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/report/asn.py
--rw-r--r--   0        0        0      105 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/report/base.py
--rw-r--r--   0        0        0      742 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/riddler.py
--rw-r--r--   0        0        0     2255 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/robots.py
--rw-r--r--   0        0        0     2578 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/secretsdb.py
--rw-r--r--   0        0        0     1071 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/securitytrails.py
--rw-r--r--   0        0        0     1198 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/shodan_dns.py
--rw-r--r--   0        0        0     1432 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/skymem.py
--rw-r--r--   0        0        0     1607 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/smuggler.py
--rw-r--r--   0        0        0     1527 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/social.py
--rw-r--r--   0        0        0     8014 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/sslcert.py
--rw-r--r--   0        0        0     6077 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/subdomain_hijack.py
--rw-r--r--   0        0        0      507 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/sublist3r.py
--rw-r--r--   0        0        0    11235 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/telerik.py
--rw-r--r--   0        0        0      566 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/threatminer.py
--rw-r--r--   0        0        0     3819 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/url_manipulation.py
--rw-r--r--   0        0        0     2759 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/urlscan.py
--rw-r--r--   0        0        0     2458 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/viewdns.py
--rw-r--r--   0        0        0     1158 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/virustotal.py
--rw-r--r--   0        0        0     1569 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/wafw00f.py
--rw-r--r--   0        0        0     1169 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/wappalyzer.py
--rw-r--r--   0        0        0     2190 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/wayback.py
--rw-r--r--   0        0        0     2095 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/modules/zoomeye.py
--rw-r--r--   0        0        0       29 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/scanner/__init__.py
--rw-r--r--   0        0        0      427 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/scanner/dispatcher.py
--rw-r--r--   0        0        0    26114 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/scanner/manager.py
--rw-r--r--   0        0        0    22025 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/scanner/scanner.py
--rw-r--r--   0        0        0     3251 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/scanner/stats.py
--rw-r--r--   0        0        0     4038 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/scanner/target.py
--rw-r--r--   0        0        0        0 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/__init__.py
--rw-r--r--   0        0        0    18609 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/bbot_fixtures.py
--rw-r--r--   0        0        0      559 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/conftest.py
--rw-r--r--   0        0        0     2545 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/helpers.py
--rw-r--r--   0        0        0    74299 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/modules_test_classes.py
--rw-r--r--   0        0        0       15 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/pytest.ini
--rwxr-xr-x   0        0        0      578 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/run_tests.sh
--rw-r--r--   0        0        0      904 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test.conf
--rw-r--r--   0        0        0      322 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_output.json
--rw-r--r--   0        0        0        0 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_1/__init__.py
--rw-r--r--   0        0        0     1397 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_1/test_before_patching.py
--rw-r--r--   0        0        0     5859 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_1/test_modules_full.py
--rw-r--r--   0        0        0        0 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/__init__.py
--rw-r--r--   0        0        0      588 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_agent.py
--rw-r--r--   0        0        0     4739 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_cli.py
--rw-r--r--   0        0        0      932 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_cloud_helpers.py
--rw-r--r--   0        0        0      462 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_config.py
--rw-r--r--   0        0        0      722 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_depsinstaller.py
--rw-r--r--   0        0        0    15064 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_events.py
--rw-r--r--   0        0        0    34798 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_helpers.py
--rw-r--r--   0        0        0     7171 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_manager.py
--rw-r--r--   0        0        0    11616 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_modules_basic.py
--rw-r--r--   0        0        0      789 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_python_api.py
--rw-r--r--   0        0        0     3215 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_scan.py
--rw-r--r--   0        0        0     1395 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_scope.py
--rw-r--r--   0        0        0     2163 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_target.py
--rw-r--r--   0        0        0      707 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_threadpool.py
--rw-r--r--   0        0        0      476 2023-04-26 15:26:56.503322 bbot-1.0.5.1656rc0/bbot/wordlists/devops_mutations.txt
--rw-r--r--   0        0        0   959424 2023-04-26 15:26:56.511322 bbot-1.0.5.1656rc0/bbot/wordlists/ffuf_shortname_candidates.txt
--rw-r--r--   0        0        0    32226 2023-04-26 15:26:56.511322 bbot-1.0.5.1656rc0/bbot/wordlists/nameservers.txt
--rw-r--r--   0        0        0     6068 2023-04-26 15:26:56.511322 bbot-1.0.5.1656rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
--rw-r--r--   0        0        0   570241 2023-04-26 15:26:56.511322 bbot-1.0.5.1656rc0/bbot/wordlists/wordninja_dns.txt.gz
--rw-r--r--   0        0        0     1338 2023-04-26 15:27:28.747710 bbot-1.0.5.1656rc0/pyproject.toml
--rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1656rc0/PKG-INFO
+-rw-r--r--   0        0        0    32473 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/LICENSE
+-rw-r--r--   0        0        0    51011 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/README.md
+-rw-r--r--   0        0        0      211 2023-05-01 21:04:54.560857 bbot-1.0.5.1660rc0/bbot/__init__.py
+-rw-r--r--   0        0        0       25 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/agent/__init__.py
+-rw-r--r--   0        0        0     6536 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/agent/agent.py
+-rw-r--r--   0        0        0      376 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/agent/messages.py
+-rwxr-xr-x   0        0        0    13693 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/cli.py
+-rw-r--r--   0        0        0       93 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/__init__.py
+-rw-r--r--   0        0        0     3171 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/configurator/__init__.py
+-rw-r--r--   0        0        0     8920 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/configurator/args.py
+-rw-r--r--   0        0        0     4261 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/configurator/environ.py
+-rw-r--r--   0        0        0     1170 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/configurator/files.py
+-rw-r--r--   0        0        0      632 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/errors.py
+-rw-r--r--   0        0        0      104 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/event/__init__.py
+-rw-r--r--   0        0        0    30371 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/event/base.py
+-rw-r--r--   0        0        0     1498 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/event/helpers.py
+-rw-r--r--   0        0        0       61 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/helpers/__init__.py
+-rw-r--r--   0        0        0     3644 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/helpers/cache.py
+-rw-r--r--   0        0        0     1256 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/aws.py
+-rw-r--r--   0        0        0      716 2023-05-01 21:04:24.904670 bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/azure.py
+-rw-r--r--   0        0        0     2875 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/base.py
+-rw-r--r--   0        0        0      297 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/digitalocean.py
+-rw-r--r--   0        0        0      271 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/firebase.py
+-rw-r--r--   0        0        0      352 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/gcp.py
+-rw-r--r--   0        0        0     6940 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/command.py
+-rw-r--r--   0        0        0       37 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/depsinstaller/__init__.py
+-rw-r--r--   0        0        0    13841 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/depsinstaller/installer.py
+-rw-r--r--   0        0        0       87 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/depsinstaller/sudo_askpass.py
+-rw-r--r--   0        0        0     8540 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/diff.py
+-rw-r--r--   0        0        0    29454 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/dns.py
+-rw-r--r--   0        0        0     4286 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/helper.py
+-rw-r--r--   0        0        0     5435 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/interactsh.py
+-rw-r--r--   0        0        0     1414 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/logger.py
+-rw-r--r--   0        0        0    29037 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/misc.py
+-rw-r--r--   0        0        0    14848 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/modules.py
+-rw-r--r--   0        0        0     9574 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/names_generator.py
+-rw-r--r--   0        0        0     2578 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/ntlm.py
+-rw-r--r--   0        0        0      795 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/punycode.py
+-rw-r--r--   0        0        0     2919 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/queueing.py
+-rw-r--r--   0        0        0     1890 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/regexes.py
+-rw-r--r--   0        0        0     8474 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/threadpool.py
+-rw-r--r--   0        0        0     3987 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/url.py
+-rw-r--r--   0        0        0     3193 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/validators.py
+-rw-r--r--   0        0        0     9324 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/web.py
+-rw-r--r--   0        0        0    10967 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/helpers/wordcloud.py
+-rw-r--r--   0        0        0       99 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/logger/__init__.py
+-rw-r--r--   0        0        0     7859 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/core/logger/logger.py
+-rw-r--r--   0        0        0     2091 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/db/neo4j.py
+-rw-r--r--   0        0        0     3731 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/defaults.yml
+-rw-r--r--   0        0        0      396 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/modules/__init__.py
+-rw-r--r--   0        0        0     1371 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/modules/anubisdb.py
+-rw-r--r--   0        0        0     3461 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/modules/azure_tenant.py
+-rw-r--r--   0        0        0     2350 2023-05-01 21:04:24.908670 bbot-1.0.5.1660rc0/bbot/modules/badsecrets.py
+-rw-r--r--   0        0        0    26022 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/base.py
+-rw-r--r--   0        0        0     2197 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/bevigil.py
+-rw-r--r--   0        0        0     1225 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/binaryedge.py
+-rw-r--r--   0        0        0     5502 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/bucket_aws.py
+-rw-r--r--   0        0        0     1065 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/bucket_azure.py
+-rw-r--r--   0        0        0      847 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/bucket_digitalocean.py
+-rw-r--r--   0        0        0     1167 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/bucket_firebase.py
+-rw-r--r--   0        0        0     2169 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/bucket_gcp.py
+-rw-r--r--   0        0        0     4550 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/builtwith.py
+-rw-r--r--   0        0        0     5107 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/bypass403.py
+-rw-r--r--   0        0        0     1116 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/c99.py
+-rw-r--r--   0        0        0     5432 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/censys.py
+-rw-r--r--   0        0        0      732 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/certspotter.py
+-rw-r--r--   0        0        0     5001 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/crobat.py
+-rw-r--r--   0        0        0     1160 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/crt.py
+-rw-r--r--   0        0        0    13578 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/deadly/ffuf.py
+-rw-r--r--   0        0        0    15617 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/deadly/nuclei.py
+-rw-r--r--   0        0        0     5763 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/deadly/vhost.py
+-rw-r--r--   0        0        0     2516 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/dnscommonsrv.py
+-rw-r--r--   0        0        0     2954 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/dnsdumpster.py
+-rw-r--r--   0        0        0     2862 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/dnszonetransfer.py
+-rw-r--r--   0        0        0      866 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/emailformat.py
+-rw-r--r--   0        0        0    11117 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/ffuf_shortnames.py
+-rw-r--r--   0        0        0     2164 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/fingerprintx.py
+-rw-r--r--   0        0        0     1093 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/fullhunt.py
+-rw-r--r--   0        0        0     7290 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/generic_ssrf.py
+-rw-r--r--   0        0        0     2723 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/github.py
+-rw-r--r--   0        0        0    10120 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/gowitness.py
+-rw-r--r--   0        0        0      658 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/hackertarget.py
+-rw-r--r--   0        0        0     7395 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/host_header.py
+-rw-r--r--   0        0        0     5546 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/httpx.py
+-rw-r--r--   0        0        0     7748 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/hunt.py
+-rw-r--r--   0        0        0     1944 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/hunterio.py
+-rw-r--r--   0        0        0     9438 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/iis_shortnames.py
+-rw-r--r--   0        0        0        0 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/internal/__init__.py
+-rw-r--r--   0        0        0      298 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/internal/aggregate.py
+-rw-r--r--   0        0        0      578 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/internal/base.py
+-rw-r--r--   0        0        0    16587 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/internal/excavate.py
+-rw-r--r--   0        0        0     4773 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/internal/speculate.py
+-rw-r--r--   0        0        0     1274 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/ipneighbor.py
+-rw-r--r--   0        0        0     2037 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/ipstack.py
+-rw-r--r--   0        0        0      707 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/leakix.py
+-rw-r--r--   0        0        0    11237 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/masscan.py
+-rw-r--r--   0        0        0    13620 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/massdns.py
+-rw-r--r--   0        0        0     4245 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/naabu.py
+-rw-r--r--   0        0        0     4867 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/ntlm.py
+-rw-r--r--   0        0        0      728 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/otx.py
+-rw-r--r--   0        0        0        0 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/__init__.py
+-rw-r--r--   0        0        0    11137 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/asset_inventory.py
+-rw-r--r--   0        0        0     1379 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/base.py
+-rw-r--r--   0        0        0     2586 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/csv.py
+-rw-r--r--   0        0        0     1809 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/http.py
+-rw-r--r--   0        0        0     1827 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/human.py
+-rw-r--r--   0        0        0     1047 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/json.py
+-rw-r--r--   0        0        0     1255 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/neo4j.py
+-rw-r--r--   0        0        0      204 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/python.py
+-rw-r--r--   0        0        0     3649 2023-05-01 21:04:24.912670 bbot-1.0.5.1660rc0/bbot/modules/output/web_report.py
+-rw-r--r--   0        0        0     1747 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/output/websocket.py
+-rw-r--r--   0        0        0     1532 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/paramminer_cookies.py
+-rw-r--r--   0        0        0     1620 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/paramminer_getparams.py
+-rw-r--r--   0        0        0     5360 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/paramminer_headers.py
+-rw-r--r--   0        0        0     1533 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/passivetotal.py
+-rw-r--r--   0        0        0     1310 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/pgp.py
+-rw-r--r--   0        0        0      746 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/rapiddns.py
+-rw-r--r--   0        0        0     1584 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/report/affiliates.py
+-rw-r--r--   0        0        0     8262 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/report/asn.py
+-rw-r--r--   0        0        0      105 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/report/base.py
+-rw-r--r--   0        0        0      742 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/riddler.py
+-rw-r--r--   0        0        0     2255 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/robots.py
+-rw-r--r--   0        0        0     2578 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/secretsdb.py
+-rw-r--r--   0        0        0     1071 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/securitytrails.py
+-rw-r--r--   0        0        0     1198 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/shodan_dns.py
+-rw-r--r--   0        0        0     1432 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/skymem.py
+-rw-r--r--   0        0        0     1607 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/smuggler.py
+-rw-r--r--   0        0        0     1527 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/social.py
+-rw-r--r--   0        0        0     8014 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/sslcert.py
+-rw-r--r--   0        0        0     6077 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/subdomain_hijack.py
+-rw-r--r--   0        0        0      507 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/sublist3r.py
+-rw-r--r--   0        0        0    11235 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/telerik.py
+-rw-r--r--   0        0        0      566 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/threatminer.py
+-rw-r--r--   0        0        0     3819 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/url_manipulation.py
+-rw-r--r--   0        0        0     2759 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/urlscan.py
+-rw-r--r--   0        0        0     2458 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/viewdns.py
+-rw-r--r--   0        0        0     1158 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/virustotal.py
+-rw-r--r--   0        0        0     1569 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/wafw00f.py
+-rw-r--r--   0        0        0     1169 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/wappalyzer.py
+-rw-r--r--   0        0        0     2190 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/wayback.py
+-rw-r--r--   0        0        0     2095 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/modules/zoomeye.py
+-rw-r--r--   0        0        0       29 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/scanner/__init__.py
+-rw-r--r--   0        0        0      427 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/scanner/dispatcher.py
+-rw-r--r--   0        0        0    26114 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/scanner/manager.py
+-rw-r--r--   0        0        0    22025 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/scanner/scanner.py
+-rw-r--r--   0        0        0     3225 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/scanner/stats.py
+-rw-r--r--   0        0        0     4038 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/scanner/target.py
+-rw-r--r--   0        0        0        0 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/__init__.py
+-rw-r--r--   0        0        0    18609 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/bbot_fixtures.py
+-rw-r--r--   0        0        0      559 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/conftest.py
+-rw-r--r--   0        0        0     2545 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/helpers.py
+-rw-r--r--   0        0        0    74299 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/modules_test_classes.py
+-rw-r--r--   0        0        0       15 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/pytest.ini
+-rwxr-xr-x   0        0        0      578 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/run_tests.sh
+-rw-r--r--   0        0        0      904 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test.conf
+-rw-r--r--   0        0        0      322 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_output.json
+-rw-r--r--   0        0        0        0 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_1/__init__.py
+-rw-r--r--   0        0        0     1397 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_1/test_before_patching.py
+-rw-r--r--   0        0        0     5859 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_1/test_modules_full.py
+-rw-r--r--   0        0        0        0 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/__init__.py
+-rw-r--r--   0        0        0      588 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_agent.py
+-rw-r--r--   0        0        0     4739 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_cli.py
+-rw-r--r--   0        0        0      932 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_cloud_helpers.py
+-rw-r--r--   0        0        0      462 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_config.py
+-rw-r--r--   0        0        0      722 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_depsinstaller.py
+-rw-r--r--   0        0        0    15064 2023-05-01 21:04:24.916670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_events.py
+-rw-r--r--   0        0        0    34798 2023-05-01 21:04:24.920670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_helpers.py
+-rw-r--r--   0        0        0     7171 2023-05-01 21:04:24.920670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_manager.py
+-rw-r--r--   0        0        0    11616 2023-05-01 21:04:24.920670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_modules_basic.py
+-rw-r--r--   0        0        0      789 2023-05-01 21:04:24.920670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_python_api.py
+-rw-r--r--   0        0        0     3215 2023-05-01 21:04:24.920670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_scan.py
+-rw-r--r--   0        0        0     1395 2023-05-01 21:04:24.920670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_scope.py
+-rw-r--r--   0        0        0     2163 2023-05-01 21:04:24.920670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_target.py
+-rw-r--r--   0        0        0      707 2023-05-01 21:04:24.920670 bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_threadpool.py
+-rw-r--r--   0        0        0      476 2023-05-01 21:04:24.920670 bbot-1.0.5.1660rc0/bbot/wordlists/devops_mutations.txt
+-rw-r--r--   0        0        0   959424 2023-05-01 21:04:24.924670 bbot-1.0.5.1660rc0/bbot/wordlists/ffuf_shortname_candidates.txt
+-rw-r--r--   0        0        0    32226 2023-05-01 21:04:24.924670 bbot-1.0.5.1660rc0/bbot/wordlists/nameservers.txt
+-rw-r--r--   0        0        0     6068 2023-05-01 21:04:24.924670 bbot-1.0.5.1660rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt
+-rw-r--r--   0        0        0   570241 2023-05-01 21:04:24.928670 bbot-1.0.5.1660rc0/bbot/wordlists/wordninja_dns.txt.gz
+-rw-r--r--   0        0        0     1338 2023-05-01 21:04:54.560857 bbot-1.0.5.1660rc0/pyproject.toml
+-rw-r--r--   0        0        0    52289 1970-01-01 00:00:00.000000 bbot-1.0.5.1660rc0/PKG-INFO
```

### Comparing `bbot-1.0.5.1656rc0/LICENSE` & `bbot-1.0.5.1660rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/README.md` & `bbot-1.0.5.1660rc0/README.md`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/agent/agent.py` & `bbot-1.0.5.1660rc0/bbot/agent/agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/cli.py` & `bbot-1.0.5.1660rc0/bbot/cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/configurator/__init__.py` & `bbot-1.0.5.1660rc0/bbot/core/configurator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/configurator/args.py` & `bbot-1.0.5.1660rc0/bbot/core/configurator/args.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/configurator/environ.py` & `bbot-1.0.5.1660rc0/bbot/core/configurator/environ.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/configurator/files.py` & `bbot-1.0.5.1660rc0/bbot/core/configurator/files.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/errors.py` & `bbot-1.0.5.1660rc0/bbot/core/errors.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/event/base.py` & `bbot-1.0.5.1660rc0/bbot/core/event/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/event/helpers.py` & `bbot-1.0.5.1660rc0/bbot/core/event/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/cache.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/__init__.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/aws.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/azure.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/cloud/base.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/cloud/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/command.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/command.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/depsinstaller/installer.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/depsinstaller/installer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/diff.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/diff.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/dns.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/helper.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/helper.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/interactsh.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/interactsh.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/logger.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/misc.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/misc.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/modules.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/modules.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/names_generator.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/names_generator.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/ntlm.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/punycode.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/punycode.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/queueing.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/queueing.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/regexes.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/regexes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/threadpool.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/url.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/url.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/validators.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/validators.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/web.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/web.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/helpers/wordcloud.py` & `bbot-1.0.5.1660rc0/bbot/core/helpers/wordcloud.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/core/logger/logger.py` & `bbot-1.0.5.1660rc0/bbot/core/logger/logger.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/db/neo4j.py` & `bbot-1.0.5.1660rc0/bbot/db/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/defaults.yml` & `bbot-1.0.5.1660rc0/bbot/defaults.yml`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/anubisdb.py` & `bbot-1.0.5.1660rc0/bbot/modules/anubisdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/azure_tenant.py` & `bbot-1.0.5.1660rc0/bbot/modules/azure_tenant.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/badsecrets.py` & `bbot-1.0.5.1660rc0/bbot/modules/badsecrets.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/base.py` & `bbot-1.0.5.1660rc0/bbot/modules/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,16 @@
     # Priority of events raised by this module, 1-5, lower numbers == higher priority
     _priority = 3
     # Name, overridden automatically
     _name = "base"
     # Type, for differentiating between normal modules and output modules, etc.
     _type = "scan"
 
+    _report_lock = threading.Lock()
+
     def __init__(self, scan):
         self.scan = scan
         self.errored = False
         self._log = None
         self._incoming_event_queue = None
         # seconds since we've submitted a batch
         self._last_submitted_batch = None
@@ -620,14 +622,28 @@
         seen = set(self.scan.pools.values())
         seen.update({self.scan, self.helpers, self.log})
         return get_size(self, max_depth=3, seen=seen)
 
     def __str__(self):
         return self.name
 
+    def log_table(self, *args, **kwargs):
+        with self._report_lock:
+            table_name = kwargs.pop("table_name", None)
+            table = self.helpers.make_table(*args, **kwargs)
+            for line in table.splitlines():
+                self.info(line)
+            if table_name is not None:
+                date = self.helpers.make_date()
+                filename = self.scan.home / f"{self.helpers.tagify(table_name)}-table-{date}.txt"
+                with open(filename, "w") as f:
+                    f.write(table)
+                self.verbose(f"Wrote {table_name} to {filename}")
+            return table
+
     def stdout(self, *args, **kwargs):
         self.log.stdout(*args, extra={"scan_id": self.scan.id}, **kwargs)
 
     def debug(self, *args, **kwargs):
         self.log.debug(*args, extra={"scan_id": self.scan.id}, **kwargs)
 
     def verbose(self, *args, **kwargs):
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/bevigil.py` & `bbot-1.0.5.1660rc0/bbot/modules/bevigil.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/binaryedge.py` & `bbot-1.0.5.1660rc0/bbot/modules/binaryedge.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/bucket_aws.py` & `bbot-1.0.5.1660rc0/bbot/modules/bucket_aws.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/bucket_azure.py` & `bbot-1.0.5.1660rc0/bbot/modules/bucket_azure.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/bucket_digitalocean.py` & `bbot-1.0.5.1660rc0/bbot/modules/bucket_digitalocean.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/bucket_firebase.py` & `bbot-1.0.5.1660rc0/bbot/modules/bucket_firebase.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/bucket_gcp.py` & `bbot-1.0.5.1660rc0/bbot/modules/bucket_gcp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/builtwith.py` & `bbot-1.0.5.1660rc0/bbot/modules/builtwith.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/bypass403.py` & `bbot-1.0.5.1660rc0/bbot/modules/bypass403.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/c99.py` & `bbot-1.0.5.1660rc0/bbot/modules/c99.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/censys.py` & `bbot-1.0.5.1660rc0/bbot/modules/censys.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/certspotter.py` & `bbot-1.0.5.1660rc0/bbot/modules/certspotter.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/crobat.py` & `bbot-1.0.5.1660rc0/bbot/modules/crobat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/crt.py` & `bbot-1.0.5.1660rc0/bbot/modules/crt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/deadly/ffuf.py` & `bbot-1.0.5.1660rc0/bbot/modules/deadly/ffuf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/deadly/nuclei.py` & `bbot-1.0.5.1660rc0/bbot/modules/deadly/nuclei.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/deadly/vhost.py` & `bbot-1.0.5.1660rc0/bbot/modules/deadly/vhost.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/dnscommonsrv.py` & `bbot-1.0.5.1660rc0/bbot/modules/dnscommonsrv.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/dnsdumpster.py` & `bbot-1.0.5.1660rc0/bbot/modules/dnsdumpster.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/dnszonetransfer.py` & `bbot-1.0.5.1660rc0/bbot/modules/dnszonetransfer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/emailformat.py` & `bbot-1.0.5.1660rc0/bbot/modules/emailformat.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/ffuf_shortnames.py` & `bbot-1.0.5.1660rc0/bbot/modules/ffuf_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/fingerprintx.py` & `bbot-1.0.5.1660rc0/bbot/modules/fingerprintx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/fullhunt.py` & `bbot-1.0.5.1660rc0/bbot/modules/fullhunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/generic_ssrf.py` & `bbot-1.0.5.1660rc0/bbot/modules/generic_ssrf.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/github.py` & `bbot-1.0.5.1660rc0/bbot/modules/github.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/gowitness.py` & `bbot-1.0.5.1660rc0/bbot/modules/gowitness.py`

 * *Files 0% similar despite different names*

```diff
@@ -239,14 +239,15 @@
             return cur.execute(query)
         except sqlite3.OperationalError as e:
             self.warning(f"Error executing query: {query}: {e}")
             self.trace()
             return []
 
     def report(self):
-        if self.screenshots_taken:
-            self.success(f"{len(self.screenshots_taken):,} web screenshots captured. To view:")
-            self.success(f"    - Start gowitness")
-            self.success(f"        - cd {self.base_path} && ./gowitness server")
-            self.success(f"    - Browse to http://localhost:7171")
-        else:
-            self.info(f"No web screenshots captured")
+        with self._report_lock:
+            if self.screenshots_taken:
+                self.success(f"{len(self.screenshots_taken):,} web screenshots captured. To view:")
+                self.success(f"    - Start gowitness")
+                self.success(f"        - cd {self.base_path} && ./gowitness server")
+                self.success(f"    - Browse to http://localhost:7171")
+            else:
+                self.info(f"No web screenshots captured")
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/hackertarget.py` & `bbot-1.0.5.1660rc0/bbot/modules/hackertarget.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/host_header.py` & `bbot-1.0.5.1660rc0/bbot/modules/host_header.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/httpx.py` & `bbot-1.0.5.1660rc0/bbot/modules/httpx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/hunt.py` & `bbot-1.0.5.1660rc0/bbot/modules/hunt.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/hunterio.py` & `bbot-1.0.5.1660rc0/bbot/modules/hunterio.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/iis_shortnames.py` & `bbot-1.0.5.1660rc0/bbot/modules/iis_shortnames.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/internal/base.py` & `bbot-1.0.5.1660rc0/bbot/modules/internal/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/internal/excavate.py` & `bbot-1.0.5.1660rc0/bbot/modules/internal/excavate.py`

 * *Files 3% similar despite different names*

```diff
@@ -331,15 +331,19 @@
                 if not scheme:
                     location_parsed = event.parsed._replace(path=location)
                     host, _ = self.helpers.split_host_port(location_parsed.netloc)
                     location = location_parsed.geturl()
                     scheme = self.helpers.is_uri(location, return_scheme=True)
                 if scheme in ("http", "https"):
                     if num_redirects <= self.max_redirects:
-                        self.emit_event(location, "URL_UNVERIFIED", event)
+                        url_event = self.make_event(location, "URL_UNVERIFIED", event)
+                        # inherit web spider distance from parent (don't increment)
+                        source_web_spider_distance = getattr(event, "web_spider_distance", 0)
+                        url_event.web_spider_distance = source_web_spider_distance
+                        self.emit_event(url_event)
                     else:
                         self.verbose(f"Exceeded max HTTP redirects ({self.max_redirects}): {location}")
                 elif scheme:
                     # we ran into a scheme that's not HTTP or HTTPS
                     data = {"host": host, "description": f"Non-standard URI scheme: {scheme}://", "url": location}
                     self.emit_event(data, "FINDING", event)
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/internal/speculate.py` & `bbot-1.0.5.1660rc0/bbot/modules/internal/speculate.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,15 +75,19 @@
                     quick=(event.type == "URL"),
                 )
 
         # generate sub-directory URLS from URLS
         if event.type == "URL":
             url_parents = self.helpers.url_parents(event.data)
             for up in url_parents:
-                self.emit_event(f"{up}/", "URL_UNVERIFIED", source=event)
+                url_event = self.make_event(f"{up}/", "URL_UNVERIFIED", source=event)
+                # inherit web spider distance from parent (don't increment)
+                source_web_spider_distance = getattr(event, "web_spider_distance", 0)
+                url_event.web_spider_distance = source_web_spider_distance
+                self.emit_event(url_event)
 
         # from hosts
         if emit_open_ports:
             # don't act on unresolved DNS_NAMEs
 
             usable_dns = False
             if event.type == "DNS_NAME":
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/ipneighbor.py` & `bbot-1.0.5.1660rc0/bbot/modules/ipneighbor.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/ipstack.py` & `bbot-1.0.5.1660rc0/bbot/modules/ipstack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/leakix.py` & `bbot-1.0.5.1660rc0/bbot/modules/leakix.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/masscan.py` & `bbot-1.0.5.1660rc0/bbot/modules/masscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/massdns.py` & `bbot-1.0.5.1660rc0/bbot/modules/massdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/naabu.py` & `bbot-1.0.5.1660rc0/bbot/modules/naabu.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/ntlm.py` & `bbot-1.0.5.1660rc0/bbot/modules/ntlm.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/otx.py` & `bbot-1.0.5.1660rc0/bbot/modules/otx.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/output/asset_inventory.py` & `bbot-1.0.5.1660rc0/bbot/modules/output/asset_inventory.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import csv
-from .csv import CSV
+import ipaddress
 
+from .csv import CSV
 from bbot.core.helpers.misc import make_ip_type, is_ip, is_port
 
 severity_map = {
     "INFO": 0,
     0: "N/A",
     1: "LOW",
     2: "MEDIUM",
@@ -18,67 +19,110 @@
 }
 
 
 class asset_inventory(CSV):
     watched_events = ["OPEN_TCP_PORT", "DNS_NAME", "URL", "FINDING", "VULNERABILITY", "TECHNOLOGY", "IP_ADDRESS"]
     produced_events = ["IP_ADDRESS", "OPEN_TCP_PORT"]
     meta = {"description": "Output to an asset inventory style flattened CSV file"}
-    options = {"output_file": "", "use_previous": False}
+    options = {"output_file": "", "use_previous": False, "summary_netmask": 16}
     options_desc = {
         "output_file": "Set a custom output file",
         "use_previous": "Emit previous asset inventory as new events (use in conjunction with -n <old_scan_name>)",
+        "summary_netmask": "Subnet mask to use when summarizing IP addresses at end of scan",
     }
 
     header_row = ["Host", "Provider", "IP(s)", "Status", "Open Ports", "Risk Rating", "Findings", "Description"]
     filename = "asset-inventory.csv"
 
     def setup(self):
         self.assets = {}
         self.open_port_producers = "httpx" in self.scan.modules or any(
             ["portscan" in m.flags for m in self.scan.modules.values()]
         )
         self.use_previous = self.config.get("use_previous", False)
+        self.summary_netmask = self.config.get("summary_netmask", 16)
         self.emitted_contents = False
         ret = super().setup()
         return ret
 
+    def filter_event(self, event):
+        if event._internal:
+            return False, "event is internal"
+        if event.type not in self.watched_events:
+            return False, "event type is not in watched_events"
+        if not self.scan.in_scope(event):
+            return False, "event is not in scope"
+        if "unresolved" in event.tags:
+            return False, "event is unresolved"
+        return True, ""
+
     def handle_event(self, event):
-        if (
-            (not event._internal)
-            and str(event.module) != "speculate"
-            and event.type in self.watched_events
-            and self.scan.in_scope(event)
-            and not "unresolved" in event.tags
-        ):
+        if self.filter_event(event)[0]:
             hostkey = _make_hostkey(event.host, event.resolved_hosts)
             if hostkey not in self.assets:
                 self.assets[hostkey] = Asset(event.host)
             self.assets[hostkey].absorb_event(event)
 
     def report(self):
+        stats = dict()
+        totals = dict()
+
+        def increment_stat(stat, value):
+            try:
+                totals[stat] += 1
+            except KeyError:
+                totals[stat] = 1
+            if not stat in stats:
+                stats[stat] = {}
+            try:
+                stats[stat][value] += 1
+            except KeyError:
+                stats[stat][value] = 1
+
         for asset in sorted(self.assets.values(), key=lambda a: str(a.host)):
             findings_and_vulns = asset.findings.union(asset.vulnerabilities)
             ports = getattr(asset, "ports", set())
             ports = [str(p) for p in sorted([int(p) for p in asset.ports])]
             ips = sorted([str(i) for i in getattr(asset, "ip_addresses", [])])
+            host = getattr(asset, "host", "")
+            if host:
+                domain = self.helpers.tldextract(host).registered_domain
+                if domain:
+                    increment_stat("Domains", domain)
+            for ip in ips:
+                net = ipaddress.ip_network(f"{ip}/{self.summary_netmask}", strict=False)
+                increment_stat("IP Addresses", str(net))
+            for port in ports:
+                increment_stat("Open Ports", port)
             row = {
-                "Host": getattr(asset, "host", ""),
+                "Host": host,
                 "Provider": getattr(asset, "provider", ""),
                 "IP(s)": ",".join(ips),
                 "Status": "Active" if asset.ports else "N/A",
                 "Open Ports": ",".join(ports),
                 "Risk Rating": severity_map[getattr(asset, "risk_rating", "")],
                 "Findings": "\n".join(findings_and_vulns),
                 "Description": "\n".join(str(x) for x in getattr(asset, "technologies", set())),
             }
             row.update(asset.custom_fields)
             self.writerow(row)
 
+        for header in ("Domains", "IP Addresses", "Open Ports"):
+            table_header = [header, ""]
+            if header in stats:
+                table = []
+                stats_sorted = sorted(stats[header].items(), key=lambda x: x[-1], reverse=True)
+                total = totals[header]
+                for k, v in stats_sorted:
+                    table.append([str(k), f"{v:,}/{total} ({v/total*100:.1f}%)"])
+                self.log_table(table, table_header, table_name=f"asset-inventory-{header}")
+
         if self._file is not None:
-            self.info(f"Saved asset-inventory output to {self.output_file}")
+            with self._report_lock:
+                self.info(f"Saved asset-inventory output to {self.output_file}")
 
     def emit_contents(self):
         if self.use_previous and not self.emitted_contents:
             self.emitted_contents = True
             if self.output_file.is_file():
                 self.info(f"Emitting previous results from {self.output_file}")
                 with open(self.output_file, newline="") as f:
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/output/base.py` & `bbot-1.0.5.1660rc0/bbot/modules/output/base.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/output/csv.py` & `bbot-1.0.5.1660rc0/bbot/modules/output/csv.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,15 +61,16 @@
     def cleanup(self):
         if getattr(self, "_file", None) is not None:
             with suppress(Exception):
                 self.file.close()
 
     def report(self):
         if self._file is not None:
-            self.info(f"Saved CSV output to {self.output_file}")
+            with self._report_lock:
+                self.info(f"Saved CSV output to {self.output_file}")
 
     def add_custom_headers(self, headers):
         if isinstance(headers, str):
             headers = [headers]
         for header in headers:
             if header not in self._headers_set:
                 self._headers_set.add(header)
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/output/http.py` & `bbot-1.0.5.1660rc0/bbot/modules/output/http.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/output/human.py` & `bbot-1.0.5.1660rc0/bbot/modules/output/human.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,8 +39,9 @@
     def cleanup(self):
         if getattr(self, "_file", None) is not None:
             with suppress(Exception):
                 self.file.close()
 
     def report(self):
         if self._file is not None:
-            self.info(f"Saved TXT output to {self.output_file}")
+            with self._report_lock:
+                self.info(f"Saved TXT output to {self.output_file}")
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/output/json.py` & `bbot-1.0.5.1660rc0/bbot/modules/output/json.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,8 +25,9 @@
     def cleanup(self):
         if getattr(self, "_file", None) is not None:
             with suppress(Exception):
                 self.file.close()
 
     def report(self):
         if self._file is not None:
-            self.info(f"Saved JSON output to {self.output_file}")
+            with self._report_lock:
+                self.info(f"Saved JSON output to {self.output_file}")
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/output/neo4j.py` & `bbot-1.0.5.1660rc0/bbot/modules/output/neo4j.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/output/web_report.py` & `bbot-1.0.5.1660rc0/bbot/modules/output/web_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,8 +89,9 @@
                 self.markdown += "\n"
 
         if self.file is not None:
             self.file.write(self.html_header)
             self.file.write(markdown.markdown(self.markdown))
             self.file.write(self.html_footer)
             self.file.flush()
-            self.info(f"Web Report saved to {self.output_file}")
+            with self._report_lock:
+                self.info(f"Web Report saved to {self.output_file}")
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/output/websocket.py` & `bbot-1.0.5.1660rc0/bbot/modules/output/websocket.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/paramminer_cookies.py` & `bbot-1.0.5.1660rc0/bbot/modules/paramminer_cookies.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/paramminer_getparams.py` & `bbot-1.0.5.1660rc0/bbot/modules/paramminer_getparams.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/paramminer_headers.py` & `bbot-1.0.5.1660rc0/bbot/modules/paramminer_headers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/passivetotal.py` & `bbot-1.0.5.1660rc0/bbot/modules/passivetotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/pgp.py` & `bbot-1.0.5.1660rc0/bbot/modules/pgp.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/rapiddns.py` & `bbot-1.0.5.1660rc0/bbot/modules/rapiddns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/report/affiliates.py` & `bbot-1.0.5.1660rc0/bbot/modules/report/affiliates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from bbot.modules.report.base import BaseReportModule
 
 
 class affiliates(BaseReportModule):
     watched_events = ["*"]
     produced_events = []
-    flags = ["passive", "safe"]
+    flags = ["passive", "safe", "affiliates"]
     meta = {"description": "Summarize affiliate domains at the end of a scan"}
     scope_distance_modifier = None
     accept_dupes = True
 
     def setup(self):
         self.affiliates = {}
         return True
@@ -20,16 +20,15 @@
         affiliates = sorted(self.affiliates.items(), key=lambda x: x[-1]["weight"], reverse=True)
         header = ["Affiliate", "Score", "Count"]
         table = []
         for domain, stats in affiliates:
             count = stats["count"]
             weight = stats["weight"]
             table.append([domain, f"{weight:.2f}", f"{count:,}"])
-        for row in self.helpers.make_table(table, header).splitlines():
-            self.info(row)
+        self.log_table(table, header, table_name="affiliates")
 
     def add_affiliate(self, event):
         if event.scope_distance > 0 and event.host and isinstance(event.host, str):
             subdomain, domain = self.helpers.split_domain(event.host)
             weight = (1 / event.scope_distance) + (1 if "affiliate" in event.tags else 0)
             if domain and not self.scan.in_scope(domain):
                 try:
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/report/asn.py` & `bbot-1.0.5.1660rc0/bbot/modules/report/asn.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,15 @@
             number = asn["asn"]
             if number != "UNKNOWN":
                 number = "AS" + number
             name = asn["name"]
             country = asn["country"]
             description = asn["description"]
             table.append([number, str(subnet), f"{count:,}", name, description, country])
-        for row in self.helpers.make_table(table, header).splitlines():
-            self.info(row)
+        self.log_table(table, header, table_name="asns")
 
     def cache_put(self, asn):
         asn = dict(asn)
         subnet = self.helpers.make_ip_type(asn.pop("subnet"))
         self.asn_cache[subnet] = asn
         try:
             self.asn_counts[subnet] += 1
```

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/riddler.py` & `bbot-1.0.5.1660rc0/bbot/modules/riddler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/robots.py` & `bbot-1.0.5.1660rc0/bbot/modules/robots.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/secretsdb.py` & `bbot-1.0.5.1660rc0/bbot/modules/secretsdb.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/securitytrails.py` & `bbot-1.0.5.1660rc0/bbot/modules/securitytrails.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/shodan_dns.py` & `bbot-1.0.5.1660rc0/bbot/modules/shodan_dns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/skymem.py` & `bbot-1.0.5.1660rc0/bbot/modules/skymem.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/smuggler.py` & `bbot-1.0.5.1660rc0/bbot/modules/smuggler.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/social.py` & `bbot-1.0.5.1660rc0/bbot/modules/social.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/sslcert.py` & `bbot-1.0.5.1660rc0/bbot/modules/sslcert.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/subdomain_hijack.py` & `bbot-1.0.5.1660rc0/bbot/modules/subdomain_hijack.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/telerik.py` & `bbot-1.0.5.1660rc0/bbot/modules/telerik.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/threatminer.py` & `bbot-1.0.5.1660rc0/bbot/modules/threatminer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/url_manipulation.py` & `bbot-1.0.5.1660rc0/bbot/modules/url_manipulation.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/urlscan.py` & `bbot-1.0.5.1660rc0/bbot/modules/urlscan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/viewdns.py` & `bbot-1.0.5.1660rc0/bbot/modules/viewdns.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/virustotal.py` & `bbot-1.0.5.1660rc0/bbot/modules/virustotal.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/wafw00f.py` & `bbot-1.0.5.1660rc0/bbot/modules/wafw00f.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/wappalyzer.py` & `bbot-1.0.5.1660rc0/bbot/modules/wappalyzer.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/wayback.py` & `bbot-1.0.5.1660rc0/bbot/modules/wayback.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/modules/zoomeye.py` & `bbot-1.0.5.1660rc0/bbot/modules/zoomeye.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/scanner/manager.py` & `bbot-1.0.5.1660rc0/bbot/scanner/manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/scanner/scanner.py` & `bbot-1.0.5.1660rc0/bbot/scanner/scanner.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/scanner/stats.py` & `bbot-1.0.5.1660rc0/bbot/scanner/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,22 @@
             if consumed:
                 consumed_str += " (" + ", ".join(f"{c:,} {t}" for t, c in consumed) + ")"
             table_row.append(consumed_str)
             table.append(table_row)
         table.sort(key=lambda x: self.module_stats[x[0]].produced_total, reverse=True)
         return [header] + table
 
-    def __str__(self):
+    def _make_table(self):
         self.perf_stats.sort(key=lambda x: x[-1])
         for callback, runtime in self.perf_stats:
             log.info(f"{callback}\t{runtime}")
         table = self.table()
         if len(table) == 1:
             table += [["None", "None", "None"]]
-        return self.scan.helpers.make_table(table[1:], table[0])
+        return table[1:], table[0]
 
 
 class ModuleStat:
     def __init__(self, module):
         self.module = module
 
         self.emitted = {}
```

### Comparing `bbot-1.0.5.1656rc0/bbot/scanner/target.py` & `bbot-1.0.5.1660rc0/bbot/scanner/target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/bbot_fixtures.py` & `bbot-1.0.5.1660rc0/bbot/test/bbot_fixtures.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/conftest.py` & `bbot-1.0.5.1660rc0/bbot/test/conftest.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/helpers.py` & `bbot-1.0.5.1660rc0/bbot/test/helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/modules_test_classes.py` & `bbot-1.0.5.1660rc0/bbot/test/modules_test_classes.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/run_tests.sh` & `bbot-1.0.5.1660rc0/bbot/test/run_tests.sh`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test.conf` & `bbot-1.0.5.1660rc0/bbot/test/test.conf`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_1/test_before_patching.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_1/test_before_patching.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_1/test_modules_full.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_1/test_modules_full.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_agent.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_agent.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_cli.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_cli.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_cloud_helpers.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_depsinstaller.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_depsinstaller.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_events.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_events.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_helpers.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_helpers.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_manager.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_manager.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_modules_basic.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_modules_basic.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_python_api.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_python_api.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_scan.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_scan.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_scope.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_scope.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_target.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_target.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/test/test_step_2/test_threadpool.py` & `bbot-1.0.5.1660rc0/bbot/test/test_step_2/test_threadpool.py`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/wordlists/ffuf_shortname_candidates.txt` & `bbot-1.0.5.1660rc0/bbot/wordlists/ffuf_shortname_candidates.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/wordlists/nameservers.txt` & `bbot-1.0.5.1660rc0/bbot/wordlists/nameservers.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt` & `bbot-1.0.5.1660rc0/bbot/wordlists/raft-small-extensions-lowercase_CLEANED.txt`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/bbot/wordlists/wordninja_dns.txt.gz` & `bbot-1.0.5.1660rc0/bbot/wordlists/wordninja_dns.txt.gz`

 * *Files identical despite different names*

### Comparing `bbot-1.0.5.1656rc0/pyproject.toml` & `bbot-1.0.5.1660rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bbot"
-version = "v1.0.5.1656rc"
+version = "v1.0.5.1660rc"
 description = "OSINT automation for hackers."
 authors = ["TheTechromancer"]
 license = "GPL-3.0"
 readme = "README.md"
 repository = "https://github.com/blacklanternsecurity/bbot"
 homepage = "https://github.com/blacklanternsecurity/bbot"
```

### Comparing `bbot-1.0.5.1656rc0/PKG-INFO` & `bbot-1.0.5.1660rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbot
-Version: 1.0.5.1656rc0
+Version: 1.0.5.1660rc0
 Summary: OSINT automation for hackers.
 Home-page: https://github.com/blacklanternsecurity/bbot
 License: GPL-3.0
 Author: TheTechromancer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

