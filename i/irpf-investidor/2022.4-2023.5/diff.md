# Comparing `tmp/irpf-investidor-2022.4.tar.gz` & `tmp/irpf_investidor-2023.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irpf-investidor-2022.4.tar", max compression
+gzip compressed data, was "irpf_investidor-2023.5.tar", max compression
```

## Comparing `irpf-investidor-2022.4.tar` & `irpf_investidor-2023.5.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1081 2022-04-21 19:28:39.085819 irpf-investidor-2022.4/LICENSE.rst
--rw-r--r--   0        0        0     5022 2022-04-21 19:28:39.085819 irpf-investidor-2022.4/README.rst
--rw-r--r--   0        0        0     1978 2022-04-21 19:28:50.369837 irpf-investidor-2022.4/pyproject.toml
--rw-r--r--   0        0        0       23 2022-04-21 19:28:39.089819 irpf-investidor-2022.4/src/irpf_investidor/__init__.py
--rw-r--r--   0        0        0     1485 2022-04-21 19:28:39.089819 irpf-investidor-2022.4/src/irpf_investidor/__main__.py
--rw-r--r--   0        0        0    26276 2022-04-21 19:28:39.089819 irpf-investidor-2022.4/src/irpf_investidor/b3.py
--rw-r--r--   0        0        0     1332 2022-04-21 19:28:39.089819 irpf-investidor-2022.4/src/irpf_investidor/formatting.py
--rw-r--r--   0        0        0     1039 2022-04-21 19:28:39.089819 irpf-investidor-2022.4/src/irpf_investidor/prompt.py
--rw-r--r--   0        0        0        0 2022-04-21 19:28:39.089819 irpf-investidor-2022.4/src/irpf_investidor/py.typed
--rw-r--r--   0        0        0     9344 2022-04-21 19:28:39.089819 irpf-investidor-2022.4/src/irpf_investidor/report_reader.py
--rw-r--r--   0        0        0     1517 2022-04-21 19:28:39.089819 irpf-investidor-2022.4/src/irpf_investidor/responses.py
--rw-r--r--   0        0        0     6040 2022-04-21 19:28:52.972985 irpf-investidor-2022.4/setup.py
--rw-r--r--   0        0        0     5963 2022-04-21 19:28:52.973536 irpf-investidor-2022.4/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-01 05:03:11.920374 irpf_investidor-2023.5/LICENSE
+-rw-r--r--   0        0        0     4628 2023-05-01 05:03:29.228535 irpf_investidor-2023.5/README.md
+-rw-r--r--   0        0        0     1888 2023-05-01 05:03:29.228535 irpf_investidor-2023.5/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/__init__.py
+-rw-r--r--   0        0        0     1449 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/__main__.py
+-rw-r--r--   0        0        0    26239 2023-05-01 05:03:29.228535 irpf_investidor-2023.5/src/irpf_investidor/b3.py
+-rw-r--r--   0        0        0     1272 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/formatting.py
+-rw-r--r--   0        0        0     1002 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/prompt.py
+-rw-r--r--   0        0        0        0 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/py.typed
+-rw-r--r--   0        0        0     9200 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/report_reader.py
+-rw-r--r--   0        0        0     1477 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/responses.py
+-rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 irpf_investidor-2023.5/PKG-INFO
```

### Comparing `irpf-investidor-2022.4/README.rst` & `irpf_investidor-2023.5/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,116 +1,90 @@
-IRPF Investidor
-===============
-
-|PyPI| |Status| |Python Version| |License|
-
-|Read the Docs| |Tests| |Codecov|
-
-|pre-commit| |Black|
-
-.. |PyPI| image:: https://img.shields.io/pypi/v/irpf-investidor.svg
-   :target: https://pypi.org/project/irpf-investidor/
-   :alt: PyPI
-.. |Status| image:: https://img.shields.io/pypi/status/irpf-investidor.svg
-   :target: https://pypi.org/project/irpf-investidor/
-   :alt: Status
-.. |Python Version| image:: https://img.shields.io/pypi/pyversions/irpf-investidor
-   :target: https://pypi.org/project/irpf-investidor
-   :alt: Python Version
-.. |License| image:: https://img.shields.io/pypi/l/irpf-investidor
-   :target: https://opensource.org/licenses/MIT
-   :alt: License
-.. |Read the Docs| image:: https://img.shields.io/readthedocs/irpf-investidor/latest.svg?label=Read%20the%20Docs
-   :target: https://irpf-investidor.readthedocs.io/
-   :alt: Read the documentation at https://irpf-investidor.readthedocs.io/
-.. |Tests| image:: https://github.com/staticdev/irpf-investidor/workflows/Tests/badge.svg
-   :target: https://github.com/staticdev/irpf-investidor/actions?workflow=Tests
-   :alt: Tests
-.. |Codecov| image:: https://codecov.io/gh/staticdev/irpf-investidor/branch/main/graph/badge.svg
-   :target: https://codecov.io/gh/staticdev/irpf-investidor
-   :alt: Codecov
-.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white
-   :target: https://github.com/pre-commit/pre-commit
-   :alt: pre-commit
-.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
-   :target: https://github.com/psf/black
-   :alt: Black
+# IRPF Investidor
 
+[![PyPI](https://img.shields.io/pypi/v/irpf-investidor.svg)][pypi status]
+[![Status](https://img.shields.io/pypi/status/irpf-investidor.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/irpf-investidor)][pypi status]
+[![License](https://img.shields.io/pypi/l/irpf-investidor)][license]
+
+[![Read the documentation at https://irpf-investidor.readthedocs.io/](https://img.shields.io/readthedocs/irpf-investidor/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/staticdev/irpf-investidor/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/staticdev/irpf-investidor/branch/main/graph/badge.svg)][codecov]
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi status]: https://pypi.org/project/irpf-investidor/
+[read the docs]: https://irpf-investidor.readthedocs.io/
+[tests]: https://github.com/staticdev/irpf-investidor/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/staticdev/irpf-investidor
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
 
 Programa auxiliar para calcular custos de ações, ETFs e FIIs. Este programa foi feito para calcular emolumentos, taxa de liquidação e custo total para a declaração de Bens e Direitos do Imposto de Renda Pessoa Física.
 
-**Essa aplicação foi testada e configurada para calcular tarifas referentes aos anos de 2019 a 2021 (IRPF 2020/2022) e não faz cálculos para compra e venda no mesmo dia (Day Trade), contratos futuros e Índice Brasil 50.**
-
+**Essa aplicação foi testada e configurada para calcular tarifas referentes aos anos de 2019 a 2022 (IRPF 2020/2023) e não faz cálculos para compra e venda no mesmo dia (Day Trade), contratos futuros e Índice Brasil 50.**
 
-Requisitos
-----------
+## Requisitos
 
 1. Python
 
-Instale na sua máquina o Python 3.8.0 ou superior (versão 3.10 recomendada) para o seu sistema operacional em python.org_.
+Instale na sua máquina o Python 3.10.0 ou superior (versão 3.10 recomendada) para o seu sistema operacional em [python.org].
 
-Usuários do Windows devem baixar a versão `Windows x86-64 executable installer` e na tela de instalação marcar a opção `Add Python 3.8 to PATH`:
+Usuários do Windows devem baixar a versão `Windows x86-64 executable installer` e na tela de instalação marcar a opção `Add Python 3.10 to PATH`:
 
-.. image:: docs/images/winpath.png
-  :width: 400
-  :alt: Checkbox PATH na instalação Windows
+```{image} docs/images/winpath.png
+:alt: "Checkbox PATH na instala\xE7\xE3o Windows"
+:width: 400
+```
 
 2. Suporte a língua Português (Brasil) no seu sistema operacional.
 
 Pode ser instalado no Linux (Debian/Ubuntu) pelo comando:
 
-.. code:: console
-
-   $ apt-get install language-pack-pt-base
+```sh
+$ apt-get install language-pack-pt-base
+```
 
+## Instalação
 
-Instalação
-----------
+You can install _IRPF Investidor_ via [pip] from [PyPI]:
 
-You can install *IRPF Investidor* via pip_ from PyPI_:
+```sh
+$ pip install irpf-investidor
+```
 
-.. code:: console
+## Uso
 
-   $ pip install irpf-investidor
+1. Entre na [Área do Investidor] da B3, faça login e entre no menu Extratos e Informativos → Negociação de Ativos → Escolha uma corretora e as datas 1 de Janeiro e 31 de Dezembro do ano em que deseja declarar. Em seguida clique no botão “Exportar para EXCEL”. Ele irá baixar o arquivo “InfoCEI.xls”.
 
-
-Uso
----
-
-1. Entre na `Área do Investidor`_ da B3, faça login e entre no menu Extratos e Informativos → Negociação de Ativos → Escolha uma corretora e as datas 1 de Janeiro e 31 de Dezembro do ano em que deseja declarar. Em seguida clique no botão “Exportar para EXCEL”. Ele irá baixar o arquivo “InfoCEI.xls”.
-
-**Ainda não é possível rodar o programa usando os novos arquivos XLSX, gerar no formato antigo.**
+**Ainda não é possível rodar o programa usando os novos arquivos XLSX, gerar no formato antigo.** Baixe e altere o [Template_InfoCEI.xls](Template_InfoCEI.xls).
 
 Você pode combinar lançamentos de anos diferentes em um mesmo documento colando as linhas de um relatório em outro, mas mantenha a ordem cronológica.
 
 2. Execute o programa através do comando:
 
-.. code:: console
-
-   $ irpf-investidor
-
+```sh
+$ irpf-investidor
+```
 
 O programa irá procurar o arquivo "InfoCEI.xls" na pasta atual (digite `pwd` no terminal para sabe qual é) ou na pasta downloads e exibirá na tela os resultados.
 
 Ao executar, o programa pede para selecionar operações realizadas em leilão. Essa informação não pode ser obtida nos relatórios da `Área do Investidor` da B3 e precisam ser buscadas diretamente com a sua corretora de valores. Isso afeta o cálculo dos emolumentos e do custo médio.
 
-
-Aviso legal (disclaimer)
-------------------------
+## Aviso legal (disclaimer)
 
 Esta é uma ferramenta com código aberto e gratuita, com licença MIT. Você pode alterar o código e distribuir, usar comercialmente como bem entender. Contribuições são muito bem vindas. Toda a responsabilidade de conferência dos valores e do envio dessas informações à Receita Federal é do usuário. Os desenvolvedores e colaboradores desse programa não se responsabilizam por quaisquer incorreções nos cálculos e lançamentos gerados.
 
+## Créditos
 
-Créditos
---------
+Esse projeto foi gerado pelo template [@cjolowicz]'s [Hypermodern Python Cookiecutter].
 
-Esse projeto foi gerado pelo template `@cjolowicz`_'s `Hypermodern Python Cookiecutter`_.
+<!-- github-only -->
 
-.. _@cjolowicz: https://github.com/cjolowicz
-.. _python.org: https://www.python.org/downloads/
-.. _Área do Investidor: https://www.investidor.b3.com.br/area-do-investidor
-.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python
-.. _PyPI: https://pypi.org/
-.. _pip: https://pip.pypa.io/
-.. github-only
-.. _Contributor Guide: CONTRIBUTING.rst
-.. _Uso: https://irpf-investidor.readthedocs.io/en/latest/usage.html
+[license]: https://github.com/staticdev/irpf-investidor/blob/main/LICENSE
+[@cjolowicz]: https://github.com/cjolowicz
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[pip]: https://pip.pypa.io/
+[pypi]: https://pypi.org/
+[python.org]: https://www.python.org/downloads/
+[uso]: https://irpf-investidor.readthedocs.io/en/latest/usage.html
+[área do investidor]: https://www.investidor.b3.com.br/
```

### Comparing `irpf-investidor-2022.4/pyproject.toml` & `irpf_investidor-2023.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,58 +1,55 @@
 [tool.poetry]
 name = "irpf-investidor"
-version = "2022.4"
+version = "2023.5"
 description = "IRPF Investidor"
-authors = ["staticdev <staticdev-support@protonmail.com>"]
+authors = ["staticdev <staticdev-support@proton.me>"]
 license = "MIT"
-readme = "README.rst"
+readme = "README.md"
 homepage = "https://github.com/staticdev/irpf-investidor"
 repository = "https://github.com/staticdev/irpf-investidor"
 documentation = "https://irpf-investidor.readthedocs.io"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/staticdev/irpf-investidor/releases"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.10"
 click = ">=8.0.1"
 pandas = ">=1.3.5"
 prompt-toolkit = ">=3.0.24"
 xlrd = ">=2.0.1"
 
 [tool.poetry.dev-dependencies]
-Pygments = ">=2.10.0"
-black = ">=21.10b0"
-coverage = {extras = ["toml"], version = ">=6.2"}
-darglint = ">=1.8.1"
-flake8 = ">=4.0.1"
-flake8-bandit = ">=2.1.2"
+bandit = ">=1.7.4"
+black = ">=22.12.0"
+coverage = {extras = ["toml"], version = ">=6.3.2"}
+flake8 = ">=5.0.4"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = ">=1.6.0"
-flake8-rst-docstrings = ">=0.2.5"
 furo = ">=2021.11.12"
 isort = ">=5.10.1"
-mypy = ">=0.930"
+mypy = ">=0.941"
 pep8-naming = ">=0.12.1"
-pre-commit = ">=2.16.0"
-pre-commit-hooks = ">=4.1.0"
-pytest = ">=6.2.5"
-pytest-mock = ">=3.6.1"
-pyupgrade = ">=2.29.1"
-safety = ">=1.10.3"
-sphinx = ">=4.3.2"
+pre-commit = ">=2.20.0"
+pre-commit-hooks = ">=4.3.0"
+pyfakefs = ">=4.5.3"
+Pygments = ">=2.11.2"
+pytest = ">=7.1.0"
+pytest-mock = ">=3.7.0"
+pyupgrade = ">=2.31.1"
+safety = ">=2.1.1"
+sphinx = ">=5.1.1"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-click = ">=3.0.2"
 typeguard = ">=2.13.3"
 xdoctest = {extras = ["colors"], version = ">=0.15.10"}
-pyfakefs = ">=4.5.3"
-bandit = "==1.7.2"
 
 [tool.poetry.scripts]
 irpf-investidor = "irpf_investidor.__main__:main"
 
 [tool.coverage.paths]
 source = ["src", "*/site-packages"]
 tests = ["tests", "*/tests"]
```

### Comparing `irpf-investidor-2022.4/src/irpf_investidor/__main__.py` & `irpf_investidor-2023.5/src/irpf_investidor/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """Command-line interface."""
-from __future__ import annotations
-
 import click
 
 import irpf_investidor.formatting
 import irpf_investidor.prompt as prompt
 import irpf_investidor.report_reader
```

### Comparing `irpf-investidor-2022.4/src/irpf_investidor/b3.py` & `irpf_investidor-2023.5/src/irpf_investidor/b3.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 """B3 module."""
-from __future__ import annotations
-
 import collections
 import datetime
 import sys
 
-
 RatePeriod = collections.namedtuple("RatePeriod", ["start_date", "end_date", "rate"])
 
 EMOLUMENTOS_PERIODS = [
     RatePeriod(
         datetime.datetime(2019, 1, 3), datetime.datetime(2019, 2, 1), 0.00004476
     ),
     RatePeriod(
@@ -66,20 +63,20 @@
     ),
     RatePeriod(
         datetime.datetime(2020, 10, 1), datetime.datetime(2020, 11, 1), 0.00003219
     ),
     RatePeriod(
         datetime.datetime(2020, 11, 1), datetime.datetime(2021, 2, 2), 0.00003247
     ),
-    RatePeriod(datetime.datetime(2021, 2, 2), datetime.datetime(2022, 1, 1), 0.00005),
+    RatePeriod(datetime.datetime(2021, 2, 2), datetime.datetime(2023, 5, 1), 0.00005),
 ]
 EMOLUMENTOS_AUCTION_RATE = 0.00007
 LIQUIDACAO_PERIODS = [
     RatePeriod(datetime.datetime(2019, 1, 3), datetime.datetime(2021, 2, 2), 0.000275),
-    RatePeriod(datetime.datetime(2021, 2, 2), datetime.datetime(2022, 1, 1), 0.00025),
+    RatePeriod(datetime.datetime(2021, 2, 2), datetime.datetime(2023, 5, 1), 0.00025),
 ]
 
 AssetInfo = collections.namedtuple("AssetInfo", ["category", "cnpj"])
 
 ETFS = {
     "BBSD": "17.817.528/0001-50",
     "XBOV": "14.120.533/0001-11",
```

### Comparing `irpf-investidor-2022.4/src/irpf_investidor/formatting.py` & `irpf_investidor-2023.5/src/irpf_investidor/formatting.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """Formatting module."""
-from __future__ import annotations
-
 import locale
 import math
-from typing import Any
-from typing import Callable
+from typing import Any, Callable
 
 import irpf_investidor.responses as res
 
 
 def set_pt_br_locale() -> res.ResponseFailure | res.ResponseSuccess:
-    """Sets pt_BR locale."""
-    # one gets available locale from shell `locale -a`
+    """Set pt_BR locale."""
+    # Get available locale from shell `locale -a`
     supported_locales = ["pt_BR.utf8", "pt_BR.UTF-8"]
     for loc in supported_locales:
         try:
             locale.setlocale(locale.LC_ALL, loc)
             return res.ResponseSuccess()
         except locale.Error:
             pass
```

### Comparing `irpf-investidor-2022.4/src/irpf_investidor/prompt.py` & `irpf_investidor-2023.5/src/irpf_investidor/prompt.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 """Prompt module."""
-from __future__ import annotations
-
 import prompt_toolkit.shortcuts as shortcuts
 
-
 TITLE = "IRPF Investidor"
 
 
 def select_trades(trades: list[tuple[int, str]]) -> list[int]:
     """Checkbox selection of auction trades.
 
     Args:
```

### Comparing `irpf-investidor-2022.4/src/irpf_investidor/report_reader.py` & `irpf_investidor-2023.5/src/irpf_investidor/report_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 """Report reader."""
-from __future__ import annotations
-
 import datetime
 import glob
 import math
 import os
 import sys
 
 import pandas as pd
 import xlrd
 
 import irpf_investidor.b3
 import irpf_investidor.formatting
 
-
 IRPF_INVESTIMENT_CODES = {
     "ETF": "74 (ETF)",
     "FII": "73 (FII)",
     "STOCKS": "31 (Ações)",
     "NOT_FOUND": "Não encontrado",
 }
 FIRST_IMPLEMENTED_YEAR = 2019
@@ -117,16 +114,14 @@
         n (float): number.
         decimals (int): Number of decimal cases. Defaults to 2.
 
     Returns:
         float: rounded number.
     """
     multiplier = 10**decimals
-    # Type-hint for floor won't work until Python 3.9
-    # https://github.com/python/typeshed/issues/3195
     return math.floor(n * multiplier) / multiplier  # type: ignore
 
 
 def clean_table_cols(source_df: pd.DataFrame) -> pd.DataFrame:
     """Drop columns without values.
 
     Args:
```

### Comparing `irpf-investidor-2022.4/src/irpf_investidor/responses.py` & `irpf_investidor-2023.5/src/irpf_investidor/responses.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 """Response objects."""
-from __future__ import annotations
-
 from typing import Any
 
 
 class ResponseTypes:
     """Response types class."""
 
     PARAMETERS_ERROR = "ParametersError"
@@ -13,15 +11,15 @@
     SUCCESS = "Success"
 
 
 class ResponseFailure:
     """Response failure class."""
 
     def __init__(self, type_: str, message: str | Exception | None) -> None:
-        """Constructor."""
+        """Construct."""
         self.type = type_
         self.message = self._format_message(message)
 
     def _format_message(self, msg: str | Exception | None) -> str | None:
         """Format message when it is an exception.
 
         Args:
@@ -48,14 +46,14 @@
         return False
 
 
 class ResponseSuccess:
     """Response success class."""
 
     def __init__(self, value: Any = None) -> None:
-        """Constructor."""
+        """Construct."""
         self.type = ResponseTypes.SUCCESS
         self.value = value
 
     def __bool__(self) -> bool:
         """Bool return for success."""
         return True
```

### Comparing `irpf-investidor-2022.4/setup.py` & `irpf_investidor-2023.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,114 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: irpf-investidor
+Version: 2023.5
+Summary: IRPF Investidor
+Home-page: https://github.com/staticdev/irpf-investidor
+License: MIT
+Author: staticdev
+Author-email: staticdev-support@proton.me
+Requires-Python: >=3.10
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (>=8.0.1)
+Requires-Dist: pandas (>=1.3.5)
+Requires-Dist: prompt-toolkit (>=3.0.24)
+Requires-Dist: xlrd (>=2.0.1)
+Project-URL: Changelog, https://github.com/staticdev/irpf-investidor/releases
+Project-URL: Documentation, https://irpf-investidor.readthedocs.io
+Project-URL: Repository, https://github.com/staticdev/irpf-investidor
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# IRPF Investidor
 
-packages = \
-['irpf_investidor']
+[![PyPI](https://img.shields.io/pypi/v/irpf-investidor.svg)][pypi status]
+[![Status](https://img.shields.io/pypi/status/irpf-investidor.svg)][pypi status]
+[![Python Version](https://img.shields.io/pypi/pyversions/irpf-investidor)][pypi status]
+[![License](https://img.shields.io/pypi/l/irpf-investidor)][license]
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['click>=8.0.1', 'pandas>=1.3.5', 'prompt-toolkit>=3.0.24', 'xlrd>=2.0.1']
-
-entry_points = \
-{'console_scripts': ['irpf-investidor = irpf_investidor.__main__:main']}
-
-setup_kwargs = {
-    'name': 'irpf-investidor',
-    'version': '2022.4',
-    'description': 'IRPF Investidor',
-    'long_description': 'IRPF Investidor\n===============\n\n|PyPI| |Status| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/irpf-investidor.svg\n   :target: https://pypi.org/project/irpf-investidor/\n   :alt: PyPI\n.. |Status| image:: https://img.shields.io/pypi/status/irpf-investidor.svg\n   :target: https://pypi.org/project/irpf-investidor/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/irpf-investidor\n   :target: https://pypi.org/project/irpf-investidor\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/irpf-investidor\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/irpf-investidor/latest.svg?label=Read%20the%20Docs\n   :target: https://irpf-investidor.readthedocs.io/\n   :alt: Read the documentation at https://irpf-investidor.readthedocs.io/\n.. |Tests| image:: https://github.com/staticdev/irpf-investidor/workflows/Tests/badge.svg\n   :target: https://github.com/staticdev/irpf-investidor/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/staticdev/irpf-investidor/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/staticdev/irpf-investidor\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n\nPrograma auxiliar para calcular custos de ações, ETFs e FIIs. Este programa foi feito para calcular emolumentos, taxa de liquidação e custo total para a declaração de Bens e Direitos do Imposto de Renda Pessoa Física.\n\n**Essa aplicação foi testada e configurada para calcular tarifas referentes aos anos de 2019 a 2021 (IRPF 2020/2022) e não faz cálculos para compra e venda no mesmo dia (Day Trade), contratos futuros e Índice Brasil 50.**\n\n\nRequisitos\n----------\n\n1. Python\n\nInstale na sua máquina o Python 3.8.0 ou superior (versão 3.10 recomendada) para o seu sistema operacional em python.org_.\n\nUsuários do Windows devem baixar a versão `Windows x86-64 executable installer` e na tela de instalação marcar a opção `Add Python 3.8 to PATH`:\n\n.. image:: docs/images/winpath.png\n  :width: 400\n  :alt: Checkbox PATH na instalação Windows\n\n2. Suporte a língua Português (Brasil) no seu sistema operacional.\n\nPode ser instalado no Linux (Debian/Ubuntu) pelo comando:\n\n.. code:: console\n\n   $ apt-get install language-pack-pt-base\n\n\nInstalação\n----------\n\nYou can install *IRPF Investidor* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install irpf-investidor\n\n\nUso\n---\n\n1. Entre na `Área do Investidor`_ da B3, faça login e entre no menu Extratos e Informativos → Negociação de Ativos → Escolha uma corretora e as datas 1 de Janeiro e 31 de Dezembro do ano em que deseja declarar. Em seguida clique no botão “Exportar para EXCEL”. Ele irá baixar o arquivo “InfoCEI.xls”.\n\n**Ainda não é possível rodar o programa usando os novos arquivos XLSX, gerar no formato antigo.**\n\nVocê pode combinar lançamentos de anos diferentes em um mesmo documento colando as linhas de um relatório em outro, mas mantenha a ordem cronológica.\n\n2. Execute o programa através do comando:\n\n.. code:: console\n\n   $ irpf-investidor\n\n\nO programa irá procurar o arquivo "InfoCEI.xls" na pasta atual (digite `pwd` no terminal para sabe qual é) ou na pasta downloads e exibirá na tela os resultados.\n\nAo executar, o programa pede para selecionar operações realizadas em leilão. Essa informação não pode ser obtida nos relatórios da `Área do Investidor` da B3 e precisam ser buscadas diretamente com a sua corretora de valores. Isso afeta o cálculo dos emolumentos e do custo médio.\n\n\nAviso legal (disclaimer)\n------------------------\n\nEsta é uma ferramenta com código aberto e gratuita, com licença MIT. Você pode alterar o código e distribuir, usar comercialmente como bem entender. Contribuições são muito bem vindas. Toda a responsabilidade de conferência dos valores e do envio dessas informações à Receita Federal é do usuário. Os desenvolvedores e colaboradores desse programa não se responsabilizam por quaisquer incorreções nos cálculos e lançamentos gerados.\n\n\nCréditos\n--------\n\nEsse projeto foi gerado pelo template `@cjolowicz`_\'s `Hypermodern Python Cookiecutter`_.\n\n.. _@cjolowicz: https://github.com/cjolowicz\n.. _python.org: https://www.python.org/downloads/\n.. _Área do Investidor: https://www.investidor.b3.com.br/area-do-investidor\n.. _Hypermodern Python Cookiecutter: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n.. _PyPI: https://pypi.org/\n.. _pip: https://pip.pypa.io/\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Uso: https://irpf-investidor.readthedocs.io/en/latest/usage.html\n',
-    'author': 'staticdev',
-    'author_email': 'staticdev-support@protonmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/staticdev/irpf-investidor',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+[![Read the documentation at https://irpf-investidor.readthedocs.io/](https://img.shields.io/readthedocs/irpf-investidor/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/staticdev/irpf-investidor/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/staticdev/irpf-investidor/branch/main/graph/badge.svg)][codecov]
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi status]: https://pypi.org/project/irpf-investidor/
+[read the docs]: https://irpf-investidor.readthedocs.io/
+[tests]: https://github.com/staticdev/irpf-investidor/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/staticdev/irpf-investidor
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+Programa auxiliar para calcular custos de ações, ETFs e FIIs. Este programa foi feito para calcular emolumentos, taxa de liquidação e custo total para a declaração de Bens e Direitos do Imposto de Renda Pessoa Física.
+
+**Essa aplicação foi testada e configurada para calcular tarifas referentes aos anos de 2019 a 2022 (IRPF 2020/2023) e não faz cálculos para compra e venda no mesmo dia (Day Trade), contratos futuros e Índice Brasil 50.**
+
+## Requisitos
+
+1. Python
+
+Instale na sua máquina o Python 3.10.0 ou superior (versão 3.10 recomendada) para o seu sistema operacional em [python.org].
+
+Usuários do Windows devem baixar a versão `Windows x86-64 executable installer` e na tela de instalação marcar a opção `Add Python 3.10 to PATH`:
+
+```{image} docs/images/winpath.png
+:alt: "Checkbox PATH na instala\xE7\xE3o Windows"
+:width: 400
+```
+
+2. Suporte a língua Português (Brasil) no seu sistema operacional.
+
+Pode ser instalado no Linux (Debian/Ubuntu) pelo comando:
+
+```sh
+$ apt-get install language-pack-pt-base
+```
+
+## Instalação
+
+You can install _IRPF Investidor_ via [pip] from [PyPI]:
+
+```sh
+$ pip install irpf-investidor
+```
+
+## Uso
+
+1. Entre na [Área do Investidor] da B3, faça login e entre no menu Extratos e Informativos → Negociação de Ativos → Escolha uma corretora e as datas 1 de Janeiro e 31 de Dezembro do ano em que deseja declarar. Em seguida clique no botão “Exportar para EXCEL”. Ele irá baixar o arquivo “InfoCEI.xls”.
+
+**Ainda não é possível rodar o programa usando os novos arquivos XLSX, gerar no formato antigo.** Baixe e altere o [Template_InfoCEI.xls](Template_InfoCEI.xls).
+
+Você pode combinar lançamentos de anos diferentes em um mesmo documento colando as linhas de um relatório em outro, mas mantenha a ordem cronológica.
+
+2. Execute o programa através do comando:
+
+```sh
+$ irpf-investidor
+```
+
+O programa irá procurar o arquivo "InfoCEI.xls" na pasta atual (digite `pwd` no terminal para sabe qual é) ou na pasta downloads e exibirá na tela os resultados.
+
+Ao executar, o programa pede para selecionar operações realizadas em leilão. Essa informação não pode ser obtida nos relatórios da `Área do Investidor` da B3 e precisam ser buscadas diretamente com a sua corretora de valores. Isso afeta o cálculo dos emolumentos e do custo médio.
+
+## Aviso legal (disclaimer)
+
+Esta é uma ferramenta com código aberto e gratuita, com licença MIT. Você pode alterar o código e distribuir, usar comercialmente como bem entender. Contribuições são muito bem vindas. Toda a responsabilidade de conferência dos valores e do envio dessas informações à Receita Federal é do usuário. Os desenvolvedores e colaboradores desse programa não se responsabilizam por quaisquer incorreções nos cálculos e lançamentos gerados.
+
+## Créditos
+
+Esse projeto foi gerado pelo template [@cjolowicz]'s [Hypermodern Python Cookiecutter].
+
+<!-- github-only -->
+
+[license]: https://github.com/staticdev/irpf-investidor/blob/main/LICENSE
+[@cjolowicz]: https://github.com/cjolowicz
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[pip]: https://pip.pypa.io/
+[pypi]: https://pypi.org/
+[python.org]: https://www.python.org/downloads/
+[uso]: https://irpf-investidor.readthedocs.io/en/latest/usage.html
+[área do investidor]: https://www.investidor.b3.com.br/
 
-setup(**setup_kwargs)
```

