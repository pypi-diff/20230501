# Comparing `tmp/cfscanner-1.3.14.tar.gz` & `tmp/cfscanner-1.3.15.tar.gz`

## Comparing `cfscanner-1.3.14.tar` & `cfscanner-1.3.15.tar`

### file list

```diff
@@ -1,44 +1,560 @@
--rw-r--r--   0        0        0    15834 2020-02-02 00:00:00.000000 cfscanner-1.3.14/temp.ipynb
--rwxr-xr-x   0        0        0 25346048 2020-02-02 00:00:00.000000 cfscanner-1.3.14/xray-linux-64
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cfscanner-1.3.14/.vscode/settings.json
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/__main__.py
--rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/args/__init__.py
--rw-r--r--   0        0        0     8281 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/args/parser.py
--rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/args/testconfig.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/report/__init__.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/report/colors.py
--rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/report/print.py
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/report/result.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/__init__.py
--rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/conduct.py
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/download.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/fronting.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/tools.py
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/speedtest/upload.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/subnets/__init__.py
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/subnets/cidr.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/subnets/regex.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/__init__.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/decorators.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/exceptions.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/os.py
--rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/requests.py
--rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/utils/socket.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/__init__.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/binary.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/config.py
--rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/service.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cfscanner-1.3.14/cfscanner/xray/templates.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/log/20230423_172219.log
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.14/log/20230423_172314.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.14/log/20230423_172527.log
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.14/result/20230423_172219_result.csv
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.14/result/20230423_172314_result.csv
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.14/result/20230423_172527_result.csv
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 cfscanner-1.3.14/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cfscanner-1.3.14/LICENSE
--rw-r--r--   0        0        0     8682 2020-02-02 00:00:00.000000 cfscanner-1.3.14/README.md
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 cfscanner-1.3.14/pyproject.toml
--rw-r--r--   0        0        0     9458 2020-02-02 00:00:00.000000 cfscanner-1.3.14/PKG-INFO
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.vscode/settings.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.102.167.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.106.32.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.109.164.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.109.244.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.125.182.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.132.215.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.169.7.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.170.157.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.174.240.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.183.101.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.190.145.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.200.230.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.206.227.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.215.212.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.219.230.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.227.194.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.230.28.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.246.91.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.247.64.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.250.250.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.27.158.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.32.142.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.57.211.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.72.175.json
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.16.8.3.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.11.114.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.116.111.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.135.42.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.15.217.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.185.2.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.222.223.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.229.103.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.234.107.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.235.104.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.247.228.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.4.149.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.42.10.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.47.58.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.56.79.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.80.176.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.81.26.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.82.60.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.88.212.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.17.95.96.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.10.128.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.103.231.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.104.166.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.104.237.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.129.105.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.134.19.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.136.18.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.14.75.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.143.114.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.144.224.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.173.76.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.190.52.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.200.220.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.39.220.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.4.62.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.40.50.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.40.89.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.45.52.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.71.193.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.18.87.20.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.100.89.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.101.144.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.122.54.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.136.144.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.156.232.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.179.1.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.180.136.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.186.112.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.187.184.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.208.69.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.218.1.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.218.142.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.240.189.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.242.196.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.244.250.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.3.251.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.34.68.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.35.134.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.75.119.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.85.135.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.19.99.238.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.117.95.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.13.86.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.142.215.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.142.48.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.148.231.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.151.9.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.181.114.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.201.56.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.21.111.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.213.49.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.243.149.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.251.248.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.255.229.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.5.116.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.64.17.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.66.92.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.76.183.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.20.9.79.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.192.46.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.194.71.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.198.255.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.209.139.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.211.74.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.216.169.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.220.87.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.33.129.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.35.200.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.43.108.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.48.242.json
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.5.4.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.50.0.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.55.49.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.82.191.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.21.93.170.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.11.129.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.27.148.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.31.136.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.37.132.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.38.61.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.4.136.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.45.136.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.46.60.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.51.241.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.69.145.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.75.105.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.22.76.203.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.23.113.187.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.23.113.202.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.23.96.72.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.234.158.18.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.234.158.188.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.0.25.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.0.26.json
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.0.9.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.1.69.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.129.162.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.135.109.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.145.43.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.147.189.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.152.89.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.154.5.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.155.134.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.159.105.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.160.221.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.161.123.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.170.230.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.183.89.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.189.34.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.194.105.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.200.14.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.225.78.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.24.243.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.240.161.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.243.200.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.243.211.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.37.248.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.38.166.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.38.25.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.40.218.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.48.45.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.66.191.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.66.221.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.24.84.148.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.132.207.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.145.33.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.146.10.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.171.168.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.185.186.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.188.126.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.191.127.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.193.8.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.206.52.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.21.135.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.225.41.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.230.17.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.235.38.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.248.173.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.33.15.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.35.227.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.63.151.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.64.147.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.80.38.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.92.182.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.92.198.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.25.99.169.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.1.129.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.1.133.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.101.40.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.115.85.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.122.56.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.15.132.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.15.53.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.16.107.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.192.175.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.203.169.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.206.241.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.39.113.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.41.46.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.5.173.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.52.245.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.65.143.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.75.181.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.77.102.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.8.117.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.96.222.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.97.174.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.97.199.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.97.42.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.27.98.214.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-104.31.16.49.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-141.101.115.120.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-141.101.115.27.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-154.84.175.90.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-154.85.99.84.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-159.112.235.29.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-160.153.0.89.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-162.159.1.94.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-162.159.135.145.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-162.159.27.123.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-162.159.27.139.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-162.159.36.211.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-162.159.44.254.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.10.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.100.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.108.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.109.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.112.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.124.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.125.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.128.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.131.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.14.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.140.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.143.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.147.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.151.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.153.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.157.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.159.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.165.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.167.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.17.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.172.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.173.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.176.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.178.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.18.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.180.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.185.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.188.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.190.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.202.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.203.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.204.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.205.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.207.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.208.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.209.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.212.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.219.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.22.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.226.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.23.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.231.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.232.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.24.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.242.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.247.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.25.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.250.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.253.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.26.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.28.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.29.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.30.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.35.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.44.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.46.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.50.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.52.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.53.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.59.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.60.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.65.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.66.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.69.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.7.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.71.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.73.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.74.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.78.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.79.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.85.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.88.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.45.90.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-170.114.46.36.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.106.208.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.130.85.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.133.209.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.149.1.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.150.2.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.162.23.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.165.196.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.174.148.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.202.92.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.22.100.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.229.46.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.38.67.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.42.4.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.64.82.13.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.66.41.105.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.66.45.29.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.67.110.160.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.67.111.54.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.67.123.23.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.67.170.87.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.67.214.41.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.67.232.125.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.67.32.82.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-172.67.84.174.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.104.157.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.104.233.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.104.247.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.106.18.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.106.250.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.106.38.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.106.48.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.107.174.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.107.248.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.107.29.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.148.107.35.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.176.26.143.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.0.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.1.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.10.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.103.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.11.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.12.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.13.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.14.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.15.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.16.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.17.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.18.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.19.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.2.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.20.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.21.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.22.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.227.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.23.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.24.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.25.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.26.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.27.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.28.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.29.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.3.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.30.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.31.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.32.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.33.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.34.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.35.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.36.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.37.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.38.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.39.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.4.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.40.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.41.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.42.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.43.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.44.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.45.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.46.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.47.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.48.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.49.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.5.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.50.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.51.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.52.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.53.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.54.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.55.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.56.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.57.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.58.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.59.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.6.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.60.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.61.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.62.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.7.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.8.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.18.250.9.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.193.31.201.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.201.139.68.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.221.160.208.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-185.221.160.3.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-188.42.88.218.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-188.42.88.227.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-188.42.88.252.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-188.42.89.174.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-188.42.89.54.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-191.101.251.112.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-191.101.251.190.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-193.227.99.54.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.245.221.143.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.85.23.48.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.85.59.101.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.85.59.102.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.85.59.154.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.85.59.174.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.85.59.204.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.85.59.238.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.85.59.242.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-195.85.59.44.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-198.41.202.5.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-198.41.206.100.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-198.41.211.1.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-198.41.219.1.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-203.22.223.51.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-203.23.103.248.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-203.29.53.252.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-203.29.54.250.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-203.32.120.136.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-203.32.121.234.json
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-212.110.135.202.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.131.6.151.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.142.120.146.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.142.120.218.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.159.216.165.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.159.216.189.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.159.216.243.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.159.216.97.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.159.217.194.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.159.217.45.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.85.119.207.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-45.85.119.87.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-80.94.83.70.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-89.116.250.121.json
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-89.116.250.131.json
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-89.116.250.47.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-94.140.0.105.json
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-94.140.0.14.json
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.xray-configs/config-94.140.0.140.json
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/__main__.py
+-rw-r--r--   0        0        0    12082 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/args/__init__.py
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/args/parser.py
+-rw-r--r--   0        0        0     4142 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/args/testconfig.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/report/__init__.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/report/colors.py
+-rw-r--r--   0        0        0     4906 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/report/print.py
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/report/result.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/speedtest/__init__.py
+-rw-r--r--   0        0        0     7514 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/speedtest/conduct.py
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/speedtest/download.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/speedtest/fronting.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/speedtest/tools.py
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/speedtest/upload.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/subnets/__init__.py
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/subnets/cidr.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/subnets/regex.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/utils/__init__.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/utils/decorators.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/utils/exceptions.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/utils/os.py
+-rw-r--r--   0        0        0      983 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/utils/requests.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/utils/socket.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/xray/__init__.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/xray/binary.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/xray/config.py
+-rw-r--r--   0        0        0     1346 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/xray/service.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 cfscanner-1.3.15/cfscanner/xray/templates.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230423_172219.log
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230423_172314.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230423_172527.log
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230423_173149.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230423_173206.log
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230423_173550.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230427_173645.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230427_174102.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230427_174129.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230427_174150.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230427_174203.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230427_174259.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230428_161250.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230428_161441.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230428_161529.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230428_161617.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083245.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083308.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083350.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083358.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083411.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083419.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083422.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083431.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083710.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083731.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083734.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083806.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083836.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083853.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083859.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_083946.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_084019.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_084127.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_084231.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cfscanner-1.3.15/log/20230430_084337.log
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230423_172219_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230423_172314_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230423_172527_result.csv
+-rw-r--r--   0        0        0    19444 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230423_173149_result.csv
+-rw-r--r--   0        0        0     3817 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230423_173206_result.csv
+-rw-r--r--   0        0        0    30000 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230423_173550_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230427_173645_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230427_174102_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230427_174129_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230427_174150_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230427_174203_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230427_174259_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230428_161441_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230428_161529_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230428_161617_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083245_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083308_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083350_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083358_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083411_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083419_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083422_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083431_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083710_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083731_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083734_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083806_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083836_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083853_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083859_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_083946_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_084019_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_084127_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_084231_result.csv
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cfscanner-1.3.15/result/20230430_084337_result.csv
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 cfscanner-1.3.15/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 cfscanner-1.3.15/LICENSE
+-rw-r--r--   0        0        0     8773 2020-02-02 00:00:00.000000 cfscanner-1.3.15/README.md
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 cfscanner-1.3.15/pyproject.toml
+-rw-r--r--   0        0        0     9549 2020-02-02 00:00:00.000000 cfscanner-1.3.15/PKG-INFO
```

### Comparing `cfscanner-1.3.14/cfscanner/main.py` & `cfscanner-1.3.15/cfscanner/main.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/args/parser.py` & `cfscanner-1.3.15/cfscanner/args/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         type=int,
         required=False
     )
     general_grp.add_argument(
         "--subnets", "-s",
         help="The path to the custom subnets file. Each line should be either a single ip (v4 or v6)"
         " or a subnet in cidr notation (v4 or v6). If not provided, the program will read the list of cidrs"
-        " from https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/cf.local.iplist",
+        " from https://github.com/MortezaBashsiz/CFScanner/blob/main/config/cf.local.iplist",
         type=str,
         metavar="",
         dest="subnets",
         required=False
     )
     ############################################################
     # Random scan options
@@ -95,15 +95,15 @@
     config_options = parser.add_argument_group(_title("Xray config options"))
     config_or_template = config_options.add_mutually_exclusive_group(
         required=False
     )
     config_or_template.add_argument(
         "--config", "-c",
         help="The path to the config file. For config file example,"
-        " see sudoer default config: https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/ClientConfig.json"
+        " see sudoer default config: https://github.com/MortezaBashsiz/CFScanner/blob/main/cofig/ClientConfig.json"
         " If not provided, the program will read the default sudoer config file",
         metavar="",
         dest="config_path",
         type=str,
         required=False
     )
     config_or_template.add_argument(
```

### Comparing `cfscanner-1.3.14/cfscanner/args/testconfig.py` & `cfscanner-1.3.15/cfscanner/args/testconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         test_config = cls()
 
         # load config if need be
         if not args.no_vpn and args.template_path is None:
             if args.config_path is None:
                 os.makedirs(os.path.join(SCRIPTDIR, ".tmp"), exist_ok=True)
                 download_file(
-                    url="https://raw.githubusercontent.com/MortezaBashsiz/CFScanner/main/bash/ClientConfig.json",
+                    url="https://raw.githubusercontent.com/MortezaBashsiz/CFScanner/main/config/ClientConfig.json",
                     save_path=os.path.join(SCRIPTDIR, ".tmp", "sudoer_config.json")
                 )
                 args.config_path = os.path.join(
                     SCRIPTDIR, ".tmp", "sudoer_config.json")
             with open(args.config_path, "r") as infile:
                 file_content = json.load(infile)
                 test_config.user_id = file_content["id"]
```

### Comparing `cfscanner-1.3.14/cfscanner/report/print.py` & `cfscanner-1.3.15/cfscanner/report/print.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/report/result.py` & `cfscanner-1.3.15/cfscanner/report/result.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/speedtest/conduct.py` & `cfscanner-1.3.15/cfscanner/speedtest/conduct.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/speedtest/download.py` & `cfscanner-1.3.15/cfscanner/speedtest/download.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/speedtest/fronting.py` & `cfscanner-1.3.15/cfscanner/speedtest/fronting.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/speedtest/upload.py` & `cfscanner-1.3.15/cfscanner/speedtest/upload.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/subnets/cidr.py` & `cfscanner-1.3.15/cfscanner/subnets/cidr.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,16 +143,16 @@
 
     Args:
         url_or_path (str): The url or path to the file to read the cidrs from
 
     Returns:
         list: The list of cidrs found in the file
     """
-    if urlparse(url_or_path).scheme:
-        cidrs = read_cidrs_from_url(url_or_path, timeout)
-    elif os.path.isfile(url_or_path):
+    if os.path.isfile(url_or_path):
         cidrs = read_cidrs_from_file(url_or_path)
+    elif urlparse(url_or_path).scheme:
+        cidrs = read_cidrs_from_url(url_or_path, timeout)
     else:
         raise SubnetsReadError(
             f"\"{url_or_path}\" is neither a valid url nor a file path."
         )
     return cidrs
```

### Comparing `cfscanner-1.3.14/cfscanner/utils/decorators.py` & `cfscanner-1.3.15/cfscanner/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/utils/exceptions.py` & `cfscanner-1.3.15/cfscanner/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/utils/os.py` & `cfscanner-1.3.15/cfscanner/utils/os.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/utils/requests.py` & `cfscanner-1.3.15/cfscanner/utils/requests.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/utils/socket.py` & `cfscanner-1.3.15/cfscanner/utils/socket.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/xray/__init__.py` & `cfscanner-1.3.15/cfscanner/xray/__init__.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/xray/binary.py` & `cfscanner-1.3.15/cfscanner/xray/binary.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/xray/config.py` & `cfscanner-1.3.15/cfscanner/xray/config.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/xray/service.py` & `cfscanner-1.3.15/cfscanner/xray/service.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/cfscanner/xray/templates.py` & `cfscanner-1.3.15/cfscanner/xray/templates.py`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/log/20230423_172314.log` & `cfscanner-1.3.15/log/20230423_172314.log`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/.gitignore` & `cfscanner-1.3.15/.gitignore`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/LICENSE` & `cfscanner-1.3.15/LICENSE`

 * *Files identical despite different names*

### Comparing `cfscanner-1.3.14/README.md` & `cfscanner-1.3.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -115,27 +115,27 @@
 
 #### General Options
 
 * `--threads`, `-t`: Number of threads to use for parallel scanning. Default value is 1.
 * `--tries`, `-n`: Number of times to try each IP. An IP is marked as OK if all tries are successful. Default value is 1.
 * `--subnets`, `-s`: The path to the custom subnets file. Each line should be either a single ip (v4 or v6) or a
   subnet in cidr notation (v4 or v6). If not provided, the program will
-  read the list of cidrs from [https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/cf.local.iplist](https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/cf.local.iplist).
+  read the list of cidrs from [https://github.com/MortezaBashsiz/CFScanner/blob/main/config/cf.local.iplist](https://github.com/MortezaBashsiz/CFScanner/blob/main/config/cf.local.iplist).
   
 #### Random Scan Options
 * `--sample`, `-r`: Size of the random sample to take from each subnet. The sample size can either
   be a float between 0 and 1 ($0 < s < 1$) or an integer ($ s \ge 1$). If it is a float, it will be
   interpreted as a percentage of the subnet size. If it is an integer, it
   will be interpreted as the number of ips to take from each subnet. If
   not provided, the program will take all ips from each subnet
 * `--shuffle-subnets`: If passed, the subnets will be shuffled before scanning.
 
 #### Xray Config Options
 
-* `--config`, `-c`: The path to the config file. For config file example, see [sudoer default config](https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/ClientConfig.json). If not provided, the program will read the [default sudoer config](https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/ClientConfig.json) file.
+* `--config`, `-c`: The path to the config file. For config file example, see [sudoer default config](https://github.com/MortezaBashsiz/CFScanner/blob/main/config/ClientConfig.json). If not provided, the program will read the [default sudoer config](https://github.com/MortezaBashsiz/CFScanner/blob/main/config/ClientConfig.json) file.
 * `--template`: Path to the proxy (v2ray/xray) client file template. By default vmess_ws_tls is used.
 * `--binpath`, `-b`: Path to the v2ray/xray binary file. If not provided, will use the latest compatible version of xray.
 * `--novpn`: If passed, xray/v2ray service will not be started and the program will not use vpn.
 * `--startprocess-timeout`: Maximum time (in seconds) to wait for xray/v2ray process to start. Default value is 5.
 
 #### Fronting Speed Test Options
 
@@ -224,10 +224,12 @@
 * 1.3.12
   * added setuptools to the dependencies
 * 1.3.13
   * added removal of duplicate subnets (issue [#490])
   * reduced the file size used for fronting test
 * 1.3.14
   * Fixed a bug in reading ips from url. The regex now supports single ips as well
+* 1.3.15
+  * Fixed a bug in reading subnets from file with full address in windows
 
 [python]: https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white
-[version]: https://img.shields.io/badge/Version-1.3.13-blue
+[version]: https://img.shields.io/badge/Version-1.3.15-blue
```

### Comparing `cfscanner-1.3.14/pyproject.toml` & `cfscanner-1.3.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cfscanner"
-version = "1.3.14"
+version = "1.3.15"
 authors = [
   { name="tempookian", email="tempookian@gmail.com" },
   { name="Morteza Bashsiz", email="morteza.bashsiz@gmail.com"}
 ]
 description = "Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `cfscanner-1.3.14/PKG-INFO` & `cfscanner-1.3.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfscanner
-Version: 1.3.14
+Version: 1.3.15
 Summary: Cloudflare's edge IPs scanner to locate ones that are viable for use with v2ray/xray
 Project-URL: Homepage, https://github.com/MortezaBashsiz/CFScanner/tree/main/python
 Project-URL: Bug Tracker, https://github.com/MortezaBashsiz/CFScanner/issues
 Author-email: tempookian <tempookian@gmail.com>, Morteza Bashsiz <morteza.bashsiz@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -133,27 +133,27 @@
 
 #### General Options
 
 * `--threads`, `-t`: Number of threads to use for parallel scanning. Default value is 1.
 * `--tries`, `-n`: Number of times to try each IP. An IP is marked as OK if all tries are successful. Default value is 1.
 * `--subnets`, `-s`: The path to the custom subnets file. Each line should be either a single ip (v4 or v6) or a
   subnet in cidr notation (v4 or v6). If not provided, the program will
-  read the list of cidrs from [https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/cf.local.iplist](https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/cf.local.iplist).
+  read the list of cidrs from [https://github.com/MortezaBashsiz/CFScanner/blob/main/config/cf.local.iplist](https://github.com/MortezaBashsiz/CFScanner/blob/main/config/cf.local.iplist).
   
 #### Random Scan Options
 * `--sample`, `-r`: Size of the random sample to take from each subnet. The sample size can either
   be a float between 0 and 1 ($0 < s < 1$) or an integer ($ s \ge 1$). If it is a float, it will be
   interpreted as a percentage of the subnet size. If it is an integer, it
   will be interpreted as the number of ips to take from each subnet. If
   not provided, the program will take all ips from each subnet
 * `--shuffle-subnets`: If passed, the subnets will be shuffled before scanning.
 
 #### Xray Config Options
 
-* `--config`, `-c`: The path to the config file. For config file example, see [sudoer default config](https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/ClientConfig.json). If not provided, the program will read the [default sudoer config](https://github.com/MortezaBashsiz/CFScanner/blob/main/bash/ClientConfig.json) file.
+* `--config`, `-c`: The path to the config file. For config file example, see [sudoer default config](https://github.com/MortezaBashsiz/CFScanner/blob/main/config/ClientConfig.json). If not provided, the program will read the [default sudoer config](https://github.com/MortezaBashsiz/CFScanner/blob/main/config/ClientConfig.json) file.
 * `--template`: Path to the proxy (v2ray/xray) client file template. By default vmess_ws_tls is used.
 * `--binpath`, `-b`: Path to the v2ray/xray binary file. If not provided, will use the latest compatible version of xray.
 * `--novpn`: If passed, xray/v2ray service will not be started and the program will not use vpn.
 * `--startprocess-timeout`: Maximum time (in seconds) to wait for xray/v2ray process to start. Default value is 5.
 
 #### Fronting Speed Test Options
 
@@ -242,10 +242,12 @@
 * 1.3.12
   * added setuptools to the dependencies
 * 1.3.13
   * added removal of duplicate subnets (issue [#490])
   * reduced the file size used for fronting test
 * 1.3.14
   * Fixed a bug in reading ips from url. The regex now supports single ips as well
+* 1.3.15
+  * Fixed a bug in reading subnets from file with full address in windows
 
 [python]: https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white
-[version]: https://img.shields.io/badge/Version-1.3.13-blue
+[version]: https://img.shields.io/badge/Version-1.3.15-blue
```

