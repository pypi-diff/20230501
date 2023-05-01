# Comparing `tmp/bibx-0.0.1a2.tar.gz` & `tmp/bibx-0.0.1a3.tar.gz`

## Comparing `bibx-0.0.1a2.tar` & `bibx-0.0.1a3.tar`

### file list

```diff
@@ -1,31 +1,34 @@
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bibx-0.0.1a2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bibx-0.0.1a2/Makefile
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 bibx-0.0.1a2/.github/workflows/cd.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bibx-0.0.1a2/.github/workflows/ci.yml
--rw-r--r--   0        0        0  2221838 2020-02-02 00:00:00.000000 bibx-0.0.1a2/docs/examples/bit-pattern-savedrecs.txt
--rw-r--r--   0        0        0  5022778 2020-02-02 00:00:00.000000 bibx-0.0.1a2/docs/examples/scopus.bib
--rw-r--r--   0        0        0  2955913 2020-02-02 00:00:00.000000 bibx-0.0.1a2/docs/examples/scopus.ris
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 bibx-0.0.1a2/docs/examples/single-article.txt
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/__init__.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/__main__.py
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/__init__.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/article.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/base.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/cross_ref.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/generic.py
--rw-r--r--   0        0        0    13195 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/isi.py
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/scopus.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/_entities/collection_builders/simple.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/algorithms/__init__.py
--rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 bibx-0.0.1a2/src/bibx/algorithms/sap.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bibx-0.0.1a2/tests/test_works.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bibx-0.0.1a2/tests/algorithms/test_sap.py
--rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 bibx-0.0.1a2/tests/entities/collection_builders/test_scopus.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 bibx-0.0.1a2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bibx-0.0.1a2/LICENSE
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 bibx-0.0.1a2/README.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bibx-0.0.1a2/pyproject.toml
--rw-r--r--   0        0        0     2498 2020-02-02 00:00:00.000000 bibx-0.0.1a2/PKG-INFO
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bibx-0.0.1a3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bibx-0.0.1a3/Makefile
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 bibx-0.0.1a3/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bibx-0.0.1a3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0  2221838 2020-02-02 00:00:00.000000 bibx-0.0.1a3/docs/examples/bit-pattern-savedrecs.txt
+-rw-r--r--   0        0        0  5022778 2020-02-02 00:00:00.000000 bibx-0.0.1a3/docs/examples/scopus.bib
+-rw-r--r--   0        0        0  2955913 2020-02-02 00:00:00.000000 bibx-0.0.1a3/docs/examples/scopus.ris
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 bibx-0.0.1a3/docs/examples/single-article.txt
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/__init__.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/__main__.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/__init__.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/article.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/base.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/cross_ref.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/generic.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/scopus_bib.py
+-rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/scopus_ris.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/simple.py
+-rw-r--r--   0        0        0    13199 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/wos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/algorithms/__init__.py
+-rw-r--r--   0        0        0    11115 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/algorithms/sap.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/test_works.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/algorithms/test_sap.py
+-rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/entities/collection_builders/test_scopus_bib.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/entities/collection_builders/test_scopus_ris.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/entities/collection_builders/test_wos.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 bibx-0.0.1a3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bibx-0.0.1a3/LICENSE
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 bibx-0.0.1a3/README.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bibx-0.0.1a3/pyproject.toml
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 bibx-0.0.1a3/PKG-INFO
```

### Comparing `bibx-0.0.1a2/.pre-commit-config.yaml` & `bibx-0.0.1a3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/.github/workflows/cd.yml` & `bibx-0.0.1a3/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/.github/workflows/ci.yml` & `bibx-0.0.1a3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/docs/examples/bit-pattern-savedrecs.txt` & `bibx-0.0.1a3/docs/examples/bit-pattern-savedrecs.txt`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/docs/examples/scopus.bib` & `bibx-0.0.1a3/docs/examples/scopus.bib`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/docs/examples/scopus.ris` & `bibx-0.0.1a3/docs/examples/scopus.ris`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/docs/examples/single-article.txt` & `bibx-0.0.1a3/docs/examples/single-article.txt`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/src/bibx/__main__.py` & `bibx-0.0.1a3/src/bibx/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import networkx as nx
 
-from bibx import read_scopus, read_wos
+from bibx import read_scopus_bib, read_wos
 from bibx.algorithms.sap import Sap
 
 
 def create_toy_graph() -> nx.DiGraph:
     #      a
     #      |
     #      b
@@ -19,15 +19,15 @@
     return g
 
 
 def create_real_graph() -> nx.DiGraph:
     with open("./docs/examples/bit-pattern-savedrecs.txt") as f:
         isi_collection = read_wos(f)
     with open("./docs/examples/scopus.bib") as f:
-        scopus_collection = read_scopus(f)
+        scopus_collection = read_scopus_bib(f)
     merged_collection = scopus_collection.merge(isi_collection)
     g = Sap.create_graph(merged_collection)
     g = Sap.clean_graph(g)
     return g
 
 
 if __name__ == "__main__":
```

### Comparing `bibx-0.0.1a2/src/bibx/exceptions.py` & `bibx-0.0.1a3/src/bibx/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,7 +25,16 @@
 class MissingCriticalInformation(BibXError, ValueError):
     """
     Raised when we don't have the publication year of an article.
     """
 
     def __init__(self):
         super().__init__("Article is missing some critical information")
+
+
+class InvalidScopusFile(BibXError, ValueError):
+    """
+    Raised when we find an invalid line on an scopus RIS file.
+    """
+
+    def __init__(self):
+        super().__init__("The file contains an invalid RIS line")
```

### Comparing `bibx-0.0.1a2/src/bibx/_entities/article.py` & `bibx-0.0.1a3/src/bibx/_entities/article.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,18 +9,18 @@
     title: Optional[str] = None
     journal: Optional[str] = None
     volume: Optional[str] = None
     issue: Optional[str] = None
     page: Optional[str] = None
     doi: Optional[str] = None
     _label: Optional[str] = None
-    references: Optional[List["Article"]] = field(default_factory=list)
-    keywords: Optional[List[str]] = field(default_factory=list)
-    sources: Optional[Set[str]] = field(default_factory=set)
-    extra: Optional[Mapping] = field(default_factory=dict)
+    references: List["Article"] = field(default_factory=list)
+    keywords: List[str] = field(default_factory=list)
+    sources: Set[str] = field(default_factory=set)
+    extra: Mapping = field(default_factory=dict)
 
     @property
     def key(self):
         author = self.authors[0].split(" ")[0].replace(",", "")
         year = self.year
         return f"{author}{year}".lower()
```

### Comparing `bibx-0.0.1a2/src/bibx/_entities/collection.py` & `bibx-0.0.1a3/src/bibx/_entities/collection.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/src/bibx/_entities/collection_builders/isi.py` & `bibx-0.0.1a3/src/bibx/_entities/collection_builders/wos.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     parser: Callable
     aliases: List[str]
 
     def parse(self, value: List[str]):
         return self.parser(value)
 
 
-class IsiCollectionBuilder(CollectionBuilder):
+class WosCollectionBuilder(CollectionBuilder):
     ISI_LINE_PATTERN = re.compile(
         r"^(null|.)?((?P<field>[A-Z0-9]{2})|  )( (?P<value>.*))?$"
     )
     ISI_CITATION_PATTERN = re.compile(
         r"""^(?P<AU>[^,]+),[ ]          # First author
             (?P<PY>\d{4}),[ ]           # Publication year
             (?P<J9>[^,]+)               # Journal
@@ -307,15 +307,15 @@
             volume=processed.get("volume"),
             issue=processed.get("issue"),
             page=processed.get("beginning_page"),
             doi=processed.get("DOI"),
             references=list(
                 cls._get_articles_from_references(processed.get("references"))
             ),
-            keywords=processed.get("keywords"),
+            keywords=processed.get("keywords", []),
             extra=processed,
             sources={article_as_str},
         )
 
     @classmethod
     def _parse_reference_from_str(cls, reference: str) -> Article:
         match = cls.ISI_CITATION_PATTERN.match(reference)
@@ -337,23 +337,23 @@
             sources={reference},
         )
 
     @staticmethod
     def _parse_all(article_data: Dict[str, List[str]]) -> Mapping[str, Any]:
         processed_data = {}
         for key, values in article_data.items():
-            parsed_values_dict = IsiCollectionBuilder._parse(key, values)
+            parsed_values_dict = WosCollectionBuilder._parse(key, values)
             processed_data.update(parsed_values_dict)
         return processed_data
 
     @staticmethod
     def _parse(key: str, value: List[str]) -> Dict:
         if key in {"FN", "VR", "ER"}:
             return {}
 
-        if key in IsiCollectionBuilder.FIELDS:
-            field = IsiCollectionBuilder.FIELDS[key]
+        if key in WosCollectionBuilder.FIELDS:
+            field = WosCollectionBuilder.FIELDS[key]
             parsed_value = field.parse(value)
             return {new_key: parsed_value for new_key in [field.key, *field.aliases]}
 
         logger.info(f"Found an unknown field with key {key} and value {value}")
         return {key: _ident(value)}
```

### Comparing `bibx-0.0.1a2/src/bibx/_entities/collection_builders/scopus.py` & `bibx-0.0.1a3/src/bibx/_entities/collection_builders/scopus_bib.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from bibx._entities.article import Article
 from bibx._entities.collection import Collection
 from bibx._entities.collection_builders.base import CollectionBuilder
 from bibx.exceptions import MissingCriticalInformation
 
 
-class ScopusCollectionBuilder(CollectionBuilder):
+class ScopusBibCollectionBuilder(CollectionBuilder):
     def __init__(self, *scopus_files: TextIO):
         self._files = scopus_files
         for file in self._files:
             file.seek(0)
 
     def build(self) -> Collection:
         articles = self._get_articles_from_files()
```

### Comparing `bibx-0.0.1a2/src/bibx/algorithms/sap.py` & `bibx-0.0.1a3/src/bibx/algorithms/sap.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import dataclasses
 import logging
-from typing import List, Set, Tuple
+from typing import Any, List, Set, Tuple, cast
 
 import networkx as nx
 from networkx.algorithms.community.louvain import louvain_communities
 
 from bibx import Article, Collection
 
 YEAR = "year"
@@ -17,21 +17,31 @@
 ELABORATE_SAP = "_elaborate_sap"
 ROOT_CONNECTIONS = "_root_connections"
 RAW_SAP = "_raw_sap"
 
 logger = logging.getLogger(__name__)
 
 
-def _limit(attribute: List[Tuple[str, int]], _max: int):
+def _limit(attribute: List[Tuple[Any, int]], _max: int):
     if _max is not None:
         sorted_attribute = sorted(attribute, key=lambda x: x[1], reverse=True)
         attribute = sorted_attribute[:_max]
     return attribute
 
 
+def _add_article_info(g: nx.DiGraph, article: Article):
+    for key, val in dataclasses.asdict(article).items():
+        if key in ("sources", "references") or key.startswith("_"):
+            continue
+        try:
+            g.nodes[article.key][key] = val
+        except KeyError:
+            g.add_node(article.key, **{key: val})
+
+
 class Sap:
     def __init__(
         self,
         max_roots: int = 20,
         max_leaves: int = 50,
         max_trunk: int = 20,
         min_leaf_connections: int = 3,
@@ -50,38 +60,105 @@
         self.max_roots = max_roots
         self.max_leaves = max_leaves
         self.max_trunk = max_trunk
         self.min_leaf_connections = min_leaf_connections
         self.max_leaf_age = max_leaf_age
         self.max_branch_size = max_branch_size
 
+    @staticmethod
+    def create_graph(collection: Collection) -> nx.DiGraph:
+        """
+        Creates a `networkx.DiGraph` from a `Collection`.
+
+        It uses the article label as a key and adds all the properties of the article to
+        the graph.
+
+        :param collection: a `bibx.Collection` instance.
+        :return: a `networkx.DiGraph` instance.
+        """
+        g = nx.DiGraph()
+        g.add_edges_from((u.key, v.key) for u, v in collection.citation_pairs)
+        for article in collection.articles:
+            for reference in article.references:
+                _add_article_info(g, reference)
+        for article in collection.articles:
+            _add_article_info(g, article)
+        g.remove_edges_from(nx.selfloop_edges(g))
+        return g
+
+    @staticmethod
+    def clean_graph(g: nx.DiGraph) -> nx.DiGraph:
+        """
+        Clean a graph to make it ready for the sap algorithm.
+
+        :param g: graph with unnecessary nodes
+        :return: cleaned up giant component
+        """
+        # Extract the giant component of the graph
+        giant_component_nodes = max(nx.weakly_connected_components(g), key=len)
+        giant: nx.DiGraph = g.subgraph(giant_component_nodes).copy()
+
+        # Remove nodes that cite one element and are never cited themselves
+        giant.remove_nodes_from(
+            [
+                n
+                for n in giant
+                if giant.in_degree(n) == 1 and giant.out_degree(n) == 0  # noqa  # noqa
+            ]
+        )
+
+        # Break loops
+        loops = [
+            loop for loop in nx.strongly_connected_components(giant) if len(loop) > 1
+        ]
+        for loop in loops:
+            giant.remove_edges_from([(u, v) for u in loop for v in loop])
+
+        return giant
+
+    def tree(self, graph: nx.DiGraph, clear: bool = False) -> nx.DiGraph:
+        """
+        Computes the whole tree.
+        """
+        graph = cast(nx.DiGraph, graph.copy())
+        graph = self._compute_root(graph)
+        graph = self._compute_leaves(graph)
+        graph = self._compute_sap(graph)
+        graph = self._compute_trunk(graph)
+        graph = self._compute_branches(graph)
+        if clear:
+            graph = self._clear(graph)
+        return graph
+
     def _compute_root(self, graph: nx.DiGraph) -> nx.DiGraph:
         """
         Takes in a connected graph and returns it labeled with a `root` property.
         :return: Labeled graph with the root property.
         """
-        g = graph.copy()
+        g = cast(nx.DiGraph, graph.copy())
         valid_roots = [
-            (n, g.in_degree(n)) for n in g.nodes if g.out_degree(n) == 0  # noqa
+            (n, cast(int, g.in_degree(n)))
+            for n in g.nodes
+            if g.out_degree(n) == 0  # noqa
         ]
         sorted_roots = _limit(valid_roots, self.max_roots)
         nx.set_node_attributes(g, 0, ROOT)
         for node, degree in sorted_roots:
             g.nodes[node][ROOT] = degree
         return g
 
     def _compute_leaves(self, graph: nx.DiGraph) -> nx.DiGraph:
         """
         Takes in a connected graph and returns it labeled with a `leaf` property.
         :param graph: Connected and filtered graph to work with.
         :return: Labeled graph with the leaf property.
         """
-        g = graph.copy()
+        g = cast(nx.DiGraph, graph.copy())
         try:
-            roots = [n for n, d in g.nodes(data=True) if d[ROOT] > 0]
+            roots = [n for n, d in g.nodes.items() if d[ROOT] > 0]
         except AttributeError:
             raise TypeError("It's necessary to have some roots")
         if not roots:
             raise TypeError("It's necessary to have some roots")
 
         nx.set_node_attributes(g, 0, ROOT_CONNECTIONS)
         for node in roots:
@@ -133,18 +210,18 @@
         return g
 
     @staticmethod
     def _compute_sap(graph: nx.DiGraph) -> nx.DiGraph:
         """
         Computes the sap of each node.
         """
-        g = graph.copy()
+        g = cast(nx.DiGraph, graph.copy())
         try:
-            valid_root = [n for n, d in g.nodes(data=True) if d[ROOT] > 0]
-            valid_leaves = [n for n, d in g.nodes(data=True) if d[LEAF] > 0]
+            valid_root = [n for n, d in g.nodes.items() if d[ROOT] > 0]
+            valid_leaves = [n for n, d in g.nodes.items() if d[LEAF] > 0]
         except AttributeError:
             raise TypeError("The graph needs to have a 'root' and a 'leaf' attribute")
         if not valid_root or not valid_leaves:
             raise TypeError("The graph needs to have at least some roots and leafs")
 
         nx.set_node_attributes(g, 0, RAW_SAP)
         nx.set_node_attributes(g, 0, ROOT_CONNECTIONS)
@@ -177,22 +254,20 @@
 
         return g
 
     def _compute_trunk(self, graph: nx.DiGraph) -> nx.DiGraph:
         """
         Tags leaves.
         """
-        g = graph.copy()
+        g = cast(nx.DiGraph, graph.copy())
         try:
             potential_trunk = [
-                (n, g.nodes[n][SAP])
-                for n in g.nodes
-                if g.nodes[n][ROOT] == 0
-                and g.nodes[n][LEAF] == 0
-                and g.nodes[n][SAP] > 0
+                (n, d[SAP])
+                for n, d in g.nodes.items()
+                if d[ROOT] == 0 and d[LEAF] == 0 and d[SAP] > 0
             ]
         except AttributeError:
             raise TypeError(
                 "The graph needs to have a 'root', 'leaf' and 'sap' attributes"
             )
         if not potential_trunk:
             raise TypeError("The graph needs to have at least some nodes with sap")
@@ -203,15 +278,15 @@
             g.nodes[node][TRUNK] = sap
         return g
 
     def _compute_branches(self, graph: nx.DiGraph) -> nx.DiGraph:
         """
         Tags branches.
         """
-        g = graph.copy()
+        g = cast(nx.DiGraph, graph.copy())
         undirected = g.to_undirected()
         communities: List[Set] = louvain_communities(undirected)
         branches = list(sorted(communities, key=len))[:3]
         nx.set_node_attributes(g, 0, BRANCH)
         for i, branch in enumerate(branches, start=1):
             potential_branch = [
                 (n, g.nodes[n][YEAR])
@@ -232,82 +307,7 @@
             n
             for n in graph.nodes
             if graph.nodes[n][ROOT] > 0
             and graph.nodes[n][TRUNK] > 0
             and graph.nodes[n][LEAF] > 0
         ]
         return graph.subgraph(nodes)
-
-    @staticmethod
-    def create_graph(collection: Collection) -> nx.DiGraph:
-        """
-        Creates a `networkx.DiGraph` from a `Collection`.
-
-        It uses the article label as a key and adds all the properties of the article to
-        the graph.
-
-        :param collection: a `bibx.Collection` instance.
-        :return: a `networkx.DiGraph` instance.
-        """
-        g = nx.DiGraph()
-        g.add_edges_from((u.key, v.key) for u, v in collection.citation_pairs)
-        for article in collection.articles:
-            for reference in article.references:
-                _add_article_info(g, reference)
-        for article in collection.articles:
-            _add_article_info(g, article)
-        g.remove_edges_from(nx.selfloop_edges(g))
-        return g
-
-    @staticmethod
-    def clean_graph(g: nx.DiGraph) -> nx.DiGraph:
-        """
-        Clean a graph to make it ready for the sap algorithm.
-
-        :param g: graph with unnecessary nodes
-        :return: cleaned up giant component
-        """
-        # Extract the giant component of the graph
-        giant_component_nodes = max(nx.weakly_connected_components(g), key=len)
-        giant: nx.DiGraph = g.subgraph(giant_component_nodes).copy()
-
-        # Remove nodes that cite one element and are never cited themselves
-        giant.remove_nodes_from(
-            [
-                n
-                for n in giant
-                if giant.in_degree(n) == 1 and giant.out_degree(n) == 0  # noqa  # noqa
-            ]
-        )
-
-        # Break loops
-        loops = [
-            loop for loop in nx.strongly_connected_components(giant) if len(loop) > 1
-        ]
-        for loop in loops:
-            giant.remove_edges_from([(u, v) for u in loop for v in loop])
-
-        return giant
-
-    def tree(self, graph: nx.DiGraph, clear: bool = False) -> nx.DiGraph:
-        """
-        Computes the whole tree.
-        """
-        graph = graph.copy()
-        graph = self._compute_root(graph)
-        graph = self._compute_leaves(graph)
-        graph = self._compute_sap(graph)
-        graph = self._compute_trunk(graph)
-        graph = self._compute_branches(graph)
-        if clear:
-            graph = self._clear(graph)
-        return graph
-
-
-def _add_article_info(g: nx.DiGraph, article: Article):
-    for key, val in dataclasses.asdict(article).items():
-        if key in ("sources", "references") or key.startswith("_"):
-            continue
-        try:
-            g.nodes[article.key][key] = val
-        except KeyError:
-            g.add_node(article.key, **{key: val})
```

### Comparing `bibx-0.0.1a2/tests/algorithms/test_sap.py` & `bibx-0.0.1a3/tests/algorithms/test_sap.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/tests/entities/collection_builders/test_scopus.py` & `bibx-0.0.1a3/tests/entities/collection_builders/test_scopus_bib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 
-from bibx._entities.collection_builders.scopus import ScopusCollectionBuilder
+from bibx import read_scopus_bib
 
 
 def test_scopus_works():
     file = io.StringIO(
         """
 @ARTICLE{Steblinski2022,
 author={Steblinski, P. and Blachowicz, T. and Ehrmann, A.},
@@ -28,15 +28,15 @@
 language={English},
 abbrev_source_title={J Magn Magn Mater},
 document_type={Article},
 source={Scopus},
 }
 """
     )
-    data = ScopusCollectionBuilder(file).build()
+    data = read_scopus_bib(file)
     assert len(data.articles) == 1
     (article,) = data.articles
     assert (
         article.title
         == "Analysis of the energy distribution of iron nano-spheres for bit-patterned media"
     )
     assert len(list(data.citation_pairs)) == 20
```

### Comparing `bibx-0.0.1a2/.gitignore` & `bibx-0.0.1a3/.gitignore`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/LICENSE` & `bibx-0.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/README.md` & `bibx-0.0.1a3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,16 +11,15 @@
 - More features in the roadmap...
 
 ## Example
 
 Here's how to apply the sap algorithm:
 
 ```python
-from bibx import read_scopus
-from bibx.algorithms.sap import Sap
+from bibx import read_scopus, Sap
 
 with open('./docs/examples/scopus.bib') as f:
     c = read_scopus(f)
 s = Sap()
 g = s.create_graph(c)
 g = s.clean_graph(g)
 g = s.tree(g)
```

### Comparing `bibx-0.0.1a2/pyproject.toml` & `bibx-0.0.1a3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a2/PKG-INFO` & `bibx-0.0.1a3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibx
-Version: 0.0.1a2
+Version: 0.0.1a3
 Summary: Python bibliometric tools.
 Author-email: Core of Science Team <technology@coreofscience.org>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: bibliometrics,science,text mining
 Requires-Dist: bibtexparser~=1.4.0
 Requires-Dist: networkx~=3.0
@@ -29,16 +29,15 @@
 - More features in the roadmap...
 
 ## Example
 
 Here's how to apply the sap algorithm:
 
 ```python
-from bibx import read_scopus
-from bibx.algorithms.sap import Sap
+from bibx import read_scopus, Sap
 
 with open('./docs/examples/scopus.bib') as f:
     c = read_scopus(f)
 s = Sap()
 g = s.create_graph(c)
 g = s.clean_graph(g)
 g = s.tree(g)
```

