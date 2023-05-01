# Comparing `tmp/graphcol-0.4.1.tar.gz` & `tmp/graphcol-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphcol-0.4.1.tar", max compression
+gzip compressed data, was "graphcol-0.4.2.tar", max compression
```

## Comparing `graphcol-0.4.1.tar` & `graphcol-0.4.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       22 2023-05-01 21:49:16.438078 graphcol-0.4.1/graphcol/__init__.py
--rw-r--r--   0        0        0     8412 2023-05-01 20:54:36.647593 graphcol-0.4.1/graphcol/exatos.py
--rw-r--r--   0        0        0     9339 2023-02-20 22:27:54.565982 graphcol-0.4.1/graphcol/gulosos.py
--rw-r--r--   0        0        0    31354 2023-02-21 03:24:18.161739 graphcol-0.4.1/graphcol/metaheuristicas.py
--rw-r--r--   0        0        0     2853 2023-02-20 22:27:54.565982 graphcol-0.4.1/graphcol/visual.py
--rw-r--r--   0        0        0      502 2023-05-01 21:49:06.613924 graphcol-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 graphcol-0.4.1/setup.py
--rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 graphcol-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-01 21:53:17.421851 graphcol-0.4.2/graphcol/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-01 21:53:00.049579 graphcol-0.4.2/graphcol/exatos.py
+-rw-r--r--   0        0        0     9339 2023-02-20 22:27:54.565982 graphcol-0.4.2/graphcol/gulosos.py
+-rw-r--r--   0        0        0    31354 2023-02-21 03:24:18.161739 graphcol-0.4.2/graphcol/metaheuristicas.py
+-rw-r--r--   0        0        0     2853 2023-02-20 22:27:54.565982 graphcol-0.4.2/graphcol/visual.py
+-rw-r--r--   0        0        0      502 2023-05-01 21:53:13.413788 graphcol-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      680 1970-01-01 00:00:00.000000 graphcol-0.4.2/setup.py
+-rw-r--r--   0        0        0      563 1970-01-01 00:00:00.000000 graphcol-0.4.2/PKG-INFO
```

### Comparing `graphcol-0.4.1/graphcol/exatos.py` & `graphcol-0.4.2/graphcol/exatos.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,18 @@
 from itertools import chain, combinations
 from graphcol.gulosos import Gulosos
 
 class Exatos:
 
   """
   Classe que contém a implementação dos algoritmos exatos para coloração de grafos,
+  até o momento foram implementados os algoritmos de Lawler que devolve o número 
+  cromático do grafo passado de entrada e o algoritmo Dsatur Exato que usa a heurística
+  de grau de saturação em conjunto com backtracking e branch-and-bound para buscar na 
+  árvore de soluções a solução exata do problema de coloração.
   """
     
   def cromatico_lawler(grafo):
     """
     Função que devolve o número cromático de um grafo. Como se trata de uma função de devolve o valor
     exato deve ser usada com cautela, pois para instâncias a partir de 10 vértices já é possível que
     o tempo de exeução da função ultrapasse 10 minutos. Por isso recomendamos uso em pequenas instâncias
@@ -42,98 +46,98 @@
         for conjunto_independente_maximal in conjuntos_independentes_maximais:
           conjunto_ajustado = [vertices_subgrafo[i] for i in list(conjunto_independente_maximal)]
           vertices_limpos = set(subgrafo) - set(conjunto_ajustado)
           X[subgrafo] = min(X[subgrafo], X[tuple(sorted(vertices_limpos))] + 1)
           
     return X[lista_subgrafos[(2**n_vertices)-1]]
 
-def dsatur_exato(grafo):
-  """
-  Função usada como interface do algoritmo dsatur exato, usada na
-  primeira que começa a recursão que implementa o backtracking. A coisa
-  mais importante que essa função faz é criar um primeira solução do dsatur 
-  """
-  numero_vertices = grafo.vcount()
-  lista_adjacencias = grafo.get_adjlist()
-  lista_arestas = grafo.get_edgelist()
-  primeira_coloracao = Gulosos.dsatur(grafo).vs["cor"]
-  melhor_resultado = len(set(primeira_coloracao))
-
-  def dsatur_recursao(grafo, melhor_geral, coloracao = [], vertices_coloridos = []):
+  def dsatur_exato(grafo):
     """
-    Função usada nas chamadas recursivas do Dsatur exato, funcionando como o
-    backtracking do algoritmo
+    Função usada como interface do algoritmo dsatur exato, usada na
+    primeira que começa a recursão que implementa o backtracking. A coisa
+    mais importante que essa função faz é criar um primeira solução do dsatur 
     """
+    numero_vertices = grafo.vcount()
+    lista_adjacencias = grafo.get_adjlist()
+    lista_arestas = grafo.get_edgelist()
+    primeira_coloracao = Gulosos.dsatur(grafo).vs["cor"]
+    melhor_resultado = len(set(primeira_coloracao))
+
+    def dsatur_recursao(grafo, melhor_geral, coloracao = [], vertices_coloridos = []):
+      """
+      Função usada nas chamadas recursivas do Dsatur exato, funcionando como o
+      backtracking do algoritmo
+      """
 
-    if vertices_coloridos == []:
-      vertices_coloridos = numero_vertices * [0]
-
-    melhor = melhor_geral
-    melhor_grafo = grafo.copy()
-    coloracao_original = coloracao.copy()
-    vertices_coloridos_original = vertices_coloridos.copy()
-    vertices_n_coloridos = vertices_coloridos.count(0)
-    vertices_tentados = []
-    tentativas_coloracao = 0
-
-    while tentativas_coloracao < vertices_n_coloridos:
-
-      vertices_coloridos = vertices_coloridos_original.copy()
-      coloracao = coloracao_original.copy()
-
-      if coloracao == []:
+      if vertices_coloridos == []:
         vertices_coloridos = numero_vertices * [0]
-        vertices_coloridos_auxiliar = vertices_coloridos
-        grau_saturacao = FuncAux.atualiza_grau_sat(lista_adjacencias, vertices_coloridos)
-        vertice_maior_grau = FuncAux.seleciona_vertice_dsatur(grau_saturacao, vertices_coloridos)
-        cor = {vertice_maior_grau}
-        coloracao = [cor]
-        vertices_coloridos[vertice_maior_grau] = 1
-        grafo.vs[vertice_maior_grau]['cor'] = coloracao.index(cor)
-      else:
-        grau_saturacao = FuncAux.atualiza_grau_sat(lista_adjacencias, vertices_coloridos)
-        vertice_maior_grau = FuncAux.seleciona_vertice_dsatur(grau_saturacao, vertices_coloridos, vertices_tentados)
-        for cor in coloracao:
-          if FuncAux.conjunto_independente(lista_arestas, cor.union({vertice_maior_grau})):
-            cor.add(vertice_maior_grau)
-            grafo.vs[vertice_maior_grau]['cor'] = coloracao.index(cor)
-            vertices_coloridos[vertice_maior_grau] = 1
-            break
-        if vertices_coloridos[vertice_maior_grau] == 0:
+
+      melhor = melhor_geral
+      melhor_grafo = grafo.copy()
+      coloracao_original = coloracao.copy()
+      vertices_coloridos_original = vertices_coloridos.copy()
+      vertices_n_coloridos = vertices_coloridos.count(0)
+      vertices_tentados = []
+      tentativas_coloracao = 0
+
+      while tentativas_coloracao < vertices_n_coloridos:
+
+        vertices_coloridos = vertices_coloridos_original.copy()
+        coloracao = coloracao_original.copy()
+
+        if coloracao == []:
+          vertices_coloridos = numero_vertices * [0]
+          vertices_coloridos_auxiliar = vertices_coloridos
+          grau_saturacao = FuncAux.atualiza_grau_sat(lista_adjacencias, vertices_coloridos)
+          vertice_maior_grau = FuncAux.seleciona_vertice_dsatur(grau_saturacao, vertices_coloridos)
           cor = {vertice_maior_grau}
-          coloracao.append(cor)
-          grafo.vs[vertice_maior_grau]['cor'] = coloracao.index(cor)
+          coloracao = [cor]
           vertices_coloridos[vertice_maior_grau] = 1
+          grafo.vs[vertice_maior_grau]['cor'] = coloracao.index(cor)
+        else:
+          grau_saturacao = FuncAux.atualiza_grau_sat(lista_adjacencias, vertices_coloridos)
+          vertice_maior_grau = FuncAux.seleciona_vertice_dsatur(grau_saturacao, vertices_coloridos, vertices_tentados)
+          for cor in coloracao:
+            if FuncAux.conjunto_independente(lista_arestas, cor.union({vertice_maior_grau})):
+              cor.add(vertice_maior_grau)
+              grafo.vs[vertice_maior_grau]['cor'] = coloracao.index(cor)
+              vertices_coloridos[vertice_maior_grau] = 1
+              break
+          if vertices_coloridos[vertice_maior_grau] == 0:
+            cor = {vertice_maior_grau}
+            coloracao.append(cor)
+            grafo.vs[vertice_maior_grau]['cor'] = coloracao.index(cor)
+            vertices_coloridos[vertice_maior_grau] = 1
 
-      qntd_cores = len(coloracao)
+        qntd_cores = len(coloracao)
 
-      if vertices_coloridos.count(1) < numero_vertices and qntd_cores < melhor_geral:
-        melhor, grafo = dsatur_recursao(grafo, melhor_geral, coloracao, vertices_coloridos)
-        vertices_tentados.append(vertice_maior_grau)
-        tentativas_coloracao = tentativas_coloracao+1
-        if melhor < melhor_geral:
-          melhor_geral = melhor
-          melhor_grafo = grafo.copy()
-        continue
+        if vertices_coloridos.count(1) < numero_vertices and qntd_cores < melhor_geral:
+          melhor, grafo = dsatur_recursao(grafo, melhor_geral, coloracao, vertices_coloridos)
+          vertices_tentados.append(vertice_maior_grau)
+          tentativas_coloracao = tentativas_coloracao+1
+          if melhor < melhor_geral:
+            melhor_geral = melhor
+            melhor_grafo = grafo.copy()
+          continue
 
-      if vertices_coloridos.count(1) == numero_vertices and qntd_cores < melhor_geral:
-        melhor_geral = qntd_cores
-        melhor_grafo = grafo.copy()
-        return melhor_geral, melhor_grafo
+        if vertices_coloridos.count(1) == numero_vertices and qntd_cores < melhor_geral:
+          melhor_geral = qntd_cores
+          melhor_grafo = grafo.copy()
+          return melhor_geral, melhor_grafo
 
-      if qntd_cores >= melhor:
-        vertices_tentados.append(vertice_maior_grau)
-        tentativas_coloracao = tentativas_coloracao+1
-        continue
+        if qntd_cores >= melhor:
+          vertices_tentados.append(vertice_maior_grau)
+          tentativas_coloracao = tentativas_coloracao+1
+          continue
 
-    return melhor_geral, melhor_grafo
+      return melhor_geral, melhor_grafo
 
-  melhor, grafo = dsatur_recursao(grafo, melhor_resultado)
+    melhor, grafo = dsatur_recursao(grafo, melhor_resultado)
 
-  return grafo
+    return grafo
 
 class FuncAux:
   '''
   Classe que contém funções auxiliares usadas pelos algoritmos gulosos.
   '''
   def conjunto_independente(lista_arestas, subconjunto_vertices):
     '''
```

### Comparing `graphcol-0.4.1/graphcol/gulosos.py` & `graphcol-0.4.2/graphcol/gulosos.py`

 * *Files identical despite different names*

### Comparing `graphcol-0.4.1/graphcol/metaheuristicas.py` & `graphcol-0.4.2/graphcol/metaheuristicas.py`

 * *Files identical despite different names*

### Comparing `graphcol-0.4.1/graphcol/visual.py` & `graphcol-0.4.2/graphcol/visual.py`

 * *Files identical despite different names*

### Comparing `graphcol-0.4.1/setup.py` & `graphcol-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['cairocffi>=1.3.0,<2.0.0',
  'igraph>=0.9.9,<0.10.0',
  'matplotlib>=3.6.0,<4.0.0',
  'numpy>=1.23.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'graphcol',
-    'version': '0.4.1',
+    'version': '0.4.2',
     'description': '',
     'long_description': 'None',
     'author': 'WLAraujo',
     'author_email': 'lima.wesleyaraujo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `graphcol-0.4.1/PKG-INFO` & `graphcol-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphcol
-Version: 0.4.1
+Version: 0.4.2
 Summary: 
 Author: WLAraujo
 Author-email: lima.wesleyaraujo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

