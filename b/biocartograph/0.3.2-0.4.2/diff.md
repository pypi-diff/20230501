# Comparing `tmp/biocartograph-0.3.2.tar.gz` & `tmp/biocartograph-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biocartograph-0.3.2.tar", last modified: Wed Apr  5 11:05:50 2023, max compression
+gzip compressed data, was "biocartograph-0.4.2.tar", last modified: Mon May  1 18:13:15 2023, max compression
```

## Comparing `biocartograph-0.3.2.tar` & `biocartograph-0.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-04-05 11:05:50.393123 biocartograph-0.3.2/
--rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-01-03 14:01:46.000000 biocartograph-0.3.2/LICENSE
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-04-05 11:05:50.392123 biocartograph-0.3.2/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-04-04 06:38:15.000000 biocartograph-0.3.2/README.md
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-04-05 11:05:50.392123 biocartograph-0.3.2/biocartograph.egg-info/
--rw-r--r--   0 rictjo    (1000) users      (100)     7248 2023-04-05 11:05:50.000000 biocartograph-0.3.2/biocartograph.egg-info/PKG-INFO
--rw-r--r--   0 rictjo    (1000) users      (100)      301 2023-04-05 11:05:50.000000 biocartograph-0.3.2/biocartograph.egg-info/SOURCES.txt
--rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-04-05 11:05:50.000000 biocartograph-0.3.2/biocartograph.egg-info/dependency_links.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-04-05 11:05:50.000000 biocartograph-0.3.2/biocartograph.egg-info/top_level.txt
--rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-04-05 11:05:50.393123 biocartograph-0.3.2/setup.cfg
--rw-r--r--   0 rictjo    (1000) users      (100)      910 2023-04-05 10:26:47.000000 biocartograph-0.3.2/setup.py
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-04-05 11:05:50.392123 biocartograph-0.3.2/src/
-drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-04-05 11:05:50.392123 biocartograph-0.3.2/src/biocartograph/
--rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-03-26 08:32:40.000000 biocartograph-0.3.2/src/biocartograph/__init__.py
--rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-03-26 10:38:54.000000 biocartograph-0.3.2/src/biocartograph/enrichment.py
--rw-r--r--   0 rictjo    (1000) users      (100)    17330 2023-04-05 10:26:47.000000 biocartograph-0.3.2/src/biocartograph/quantification.py
--rw-r--r--   0 rictjo    (1000) users      (100)    10708 2023-04-05 10:26:47.000000 biocartograph-0.3.2/src/biocartograph/special.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-01 18:13:15.505048 biocartograph-0.4.2/
+-rw-r--r--   0 rictjo    (1000) users      (100)    11357 2023-05-01 17:36:58.000000 biocartograph-0.4.2/LICENSE
+-rw-r--r--   0 rictjo    (1000) users      (100)     7211 2023-05-01 18:13:15.505048 biocartograph-0.4.2/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)     6705 2023-05-01 17:36:58.000000 biocartograph-0.4.2/README.md
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-01 18:13:15.504048 biocartograph-0.4.2/biocartograph.egg-info/
+-rw-r--r--   0 rictjo    (1000) users      (100)     7211 2023-05-01 18:13:15.000000 biocartograph-0.4.2/biocartograph.egg-info/PKG-INFO
+-rw-r--r--   0 rictjo    (1000) users      (100)      301 2023-05-01 18:13:15.000000 biocartograph-0.4.2/biocartograph.egg-info/SOURCES.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)        1 2023-05-01 18:13:15.000000 biocartograph-0.4.2/biocartograph.egg-info/dependency_links.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       14 2023-05-01 18:13:15.000000 biocartograph-0.4.2/biocartograph.egg-info/top_level.txt
+-rw-r--r--   0 rictjo    (1000) users      (100)       38 2023-05-01 18:13:15.505048 biocartograph-0.4.2/setup.cfg
+-rw-r--r--   0 rictjo    (1000) users      (100)      910 2023-05-01 17:37:01.000000 biocartograph-0.4.2/setup.py
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-01 18:13:15.504048 biocartograph-0.4.2/src/
+drwxr-xr-x   0 rictjo    (1000) users      (100)        0 2023-05-01 18:13:15.504048 biocartograph-0.4.2/src/biocartograph/
+-rw-r--r--   0 rictjo    (1000) users      (100)       23 2023-05-01 17:36:58.000000 biocartograph-0.4.2/src/biocartograph/__init__.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    14381 2023-05-01 17:36:58.000000 biocartograph-0.4.2/src/biocartograph/enrichment.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    18799 2023-05-01 18:09:12.000000 biocartograph-0.4.2/src/biocartograph/quantification.py
+-rw-r--r--   0 rictjo    (1000) users      (100)    14707 2023-05-01 17:37:01.000000 biocartograph-0.4.2/src/biocartograph/special.py
```

### Comparing `biocartograph-0.3.2/LICENSE` & `biocartograph-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `biocartograph-0.3.2/PKG-INFO` & `biocartograph-0.4.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.3.2
+Version: 0.4.2
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Biocartograph
@@ -147,9 +145,7 @@
 Blood Cells:
 [blood cells](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/200153c58767d8b5162e66688ff4d669/raw/cfb74069d5cc9fc58e3558c753caaa60d4ba5e9b/index.html)
 [biocartograph gfa enrichment](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/42ec85df088a0c40de339a78322594bd/raw/0725bea467b0c153298655e3a0555670a812e80f/index.html)
 [biocartograph treemap cluster 2](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/d754528cf594087e509fe44fa071c178/raw/a78a82066e3d6aa2971aba2a64543a4018241372/index.html)
 
 [TCGA-BRCA](https://gdc.cancer.gov/) :
 Calculated using the biocartograph and a [TCGA derived data set](https://zenodo.org/record/3407557) with the results for [Breast Cancer mRNA-seq](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/ea18ac756d5142ac98219d45960583d4/raw/7cba81abb8af89416d11a682a2e0d19a311c954f/index.html)
-
-
```

### Comparing `biocartograph-0.3.2/README.md` & `biocartograph-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `biocartograph-0.3.2/biocartograph.egg-info/PKG-INFO` & `biocartograph-0.4.2/biocartograph.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: biocartograph
-Version: 0.3.2
+Version: 0.4.2
 Summary: Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash
 Home-page: https://github.com/rictjo/biocarta
 Author: Richard Tjörnhammar
 Author-email: richard.tjornhammar@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Biocartograph
@@ -147,9 +145,7 @@
 Blood Cells:
 [blood cells](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/200153c58767d8b5162e66688ff4d669/raw/cfb74069d5cc9fc58e3558c753caaa60d4ba5e9b/index.html)
 [biocartograph gfa enrichment](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/42ec85df088a0c40de339a78322594bd/raw/0725bea467b0c153298655e3a0555670a812e80f/index.html)
 [biocartograph treemap cluster 2](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/d754528cf594087e509fe44fa071c178/raw/a78a82066e3d6aa2971aba2a64543a4018241372/index.html)
 
 [TCGA-BRCA](https://gdc.cancer.gov/) :
 Calculated using the biocartograph and a [TCGA derived data set](https://zenodo.org/record/3407557) with the results for [Breast Cancer mRNA-seq](https://rictjo.github.io/?https://gist.githubusercontent.com/rictjo/ea18ac756d5142ac98219d45960583d4/raw/7cba81abb8af89416d11a682a2e0d19a311c954f/index.html)
-
-
```

### Comparing `biocartograph-0.3.2/setup.py` & `biocartograph-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name         = "biocartograph",
-    version      = "0.3.2",
+    version      = "0.4.2",
     author       = "Richard Tjörnhammar",
     author_email = "richard.tjornhammar@gmail.com",
     description  = "Package was renamed from Biocarta v0.2.27 to Biocartograph because of an unintentional name clash",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://github.com/rictjo/biocarta",
     packages = setuptools.find_packages('src'),
```

### Comparing `biocartograph-0.3.2/src/biocartograph/enrichment.py` & `biocartograph-0.4.2/src/biocartograph/enrichment.py`

 * *Files identical despite different names*

### Comparing `biocartograph-0.3.2/src/biocartograph/quantification.py` & `biocartograph-0.4.2/src/biocartograph/quantification.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,17 @@
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
-import pandas as pd
-import numpy as np
+import pandas   as pd
+import numpy    as np
+import kmapper  as km # GENERAL TDA TOOLBOX
 import umap
 
 import impetuous.quantification as impq
 import impetuous.clustering     as impc
 
 from impetuous.quantification	import distance_calculation
 from impetuous.clustering	import generate_clustering_labels
@@ -28,15 +29,18 @@
                      bUseUmap:bool		= False	,
                      umap_dimension:int		= 2	,
                      n_neighbors:int		= 20	,
                      MF:np.array		= None	,
                      bNonEuclideanBackprojection:bool = False ,
                      n_proj:int			= 2	,
                      local_connectivity:float	= 20.	,
-                     Sfunc = lambda x:np.mean(x,0) ,
+                     Sfunc = lambda x:np.mean(x,0)	,
+                     bUseTDA:bool               = False ,
+                     contraction_quantile:float = None  ,
+                     contraction_depth:float    = None  ,
                      transform_seed:int = 42 ) -> tuple[pd.DataFrame] :
     #
     if MF is None :
         # IF NOT PRECOMPUTED
         # WASTE OF COMPUTATION ...
         if bNonEuclideanBackprojection :
             u , s , vt = np.linalg.svd ( distm , False )
@@ -44,22 +48,39 @@
         else :
             Xf = distance_matrix_to_absolute_coordinates ( distm ,
                 n_dimensions = -1 , bLegacy = False )
         MF = Xf
     else :
         Xf = MF
     #
-    Uf = pd.DataFrame( umap.UMAP( local_connectivity	= local_connectivity	,
+    if not contraction_quantile is None :
+        import biocartograph.special as biox
+        Xf = biox.contract( distm , quantile = contraction_quantile , d=contraction_depth )
+
+    col_label_prefix = 'UMAP.'
+    if bUseTDA :
+        from sklearn import ensemble , preprocessing, manifold
+        import kmapper as km
+        model   = ensemble.IsolationForest( random_state=1337 )
+        model   .fit( Xf )
+        lens1   = model.decision_function( Xf )
+        P	= (lens1*Xf.T).T
+        print ( 'WARNING: THIS IS A HIGHLY DEVELOPMENTAL FEATURE. TDA => KMAP' )
+        mapper  = km.KeplerMapper( verbose=0 )
+        Uf      = pd.DataFrame( mapper.fit_transform( Xf , projection = [a for a in range(int(umap_dimension)) ] ) )
+        col_label_prefix = 'TDA.'
+    else :
+        Uf = pd.DataFrame( umap.UMAP( local_connectivity	= local_connectivity	,
                                   n_components		= int(umap_dimension)	,
                                   n_neighbors		= int(n_neighbors)	,
                                   transform_seed	= transform_seed	,
                                     ) .fit_transform( Xf ) )
-    resdf = pd.DataFrame( Uf )
-    resdf .index = index_labels
-    resdf .columns = ['UMAP.'+str(i) for i in range(umap_dimension)]
+    resdf		= pd.DataFrame( Uf )
+    resdf .index	= index_labels
+    resdf .columns	= [ col_label_prefix + str(i) for i in range(umap_dimension)]
     #
     if bUseUmap :
         distm = distance_calculation ( Uf , 'euclidean' ,
                              bRemoveCurse = True , nRound = None )
     if not n_clusters is None :
         n_cl = n_clusters[0]
     else :
@@ -93,22 +114,24 @@
     #
     return ( resdf, hierarch_df , pd.DataFrame(sol) )
 
 
 def full_mapping ( adf:pd.DataFrame , jdf:pd.DataFrame ,
         bVerbose:bool = True , bExtreme:bool = True , n_clusters:list[int] = None ,
         n_components:int = None , bUseUmap:bool = False , bPreCompute:bool=True ,
-        distance_type:str  = 'covariation' , # 'correlation,spearman,absolute' ,
-        umap_dimension:int = 2 , umap_n_neighbors:int = 20 , umap_local_connectivity:float = 1. ,
-        umap_seed:int = 42 , hierarchy_cmd:str = 'max' , divergence = lambda r : np.exp(r) ,
+        distance_type:str  = 'covariation' ,
+        umap_dimension:int = 2 , umap_n_neighbors:int = 20 , umap_local_connectivity:float = 20. ,
+        umap_seed:int = 42 , hierarchy_cmd:str = 'ward' , divergence = lambda r : np.exp(r) ,
         add_labels:list[str] = None , sample_label:str = None , alignment_label:str = None , bRemoveCurse:bool=False ,
         n_projections:int = 2 , directory:str = './' , bQN:int = None ,
         nNeighborFilter:list[int] = None , heal_symmetry_break_method:str = 'average' ,
         epls_ownership:str = 'angle' , bNonEuclideanBackprojection:bool = False ,
-        Sfunc = lambda x:np.mean(x,0) , bAddPies:bool=False ) -> tuple[pd.DataFrame] :
+        Sfunc = lambda x:np.mean(x,0) , bAddPies:bool=False , bUseTDA:bool = False ,
+        contraction_quantile:float = None   ,
+        contraction_depth:float    = None   ) -> tuple[pd.DataFrame] :
     #
     import biocartograph.special as biox
     #
     if bVerbose :
         print ( "TO DISABLE WRITING OF RESULTS TO", directory )
         print ( "SET THE directory=None " )
         print ( "TO MAKE BIOCARTOGRAPH QUIET SET bVerbose=False" )
@@ -128,15 +151,16 @@
         'n_components:int':n_components , 'bUseUmap:bool':bUseUmap , 'bPreCompute:bool':bPreCompute , 'distance_type:str':distance_type ,
         'umap_dimension:int':umap_dimension , 'umap_n_neighbors:int':umap_n_neighbors , 'umap_local_connectivity:float':umap_local_connectivity ,
         'umap_seed:int':umap_seed , 'hierarchy_cmd:str':hierarchy_cmd , 'divergence:lambda function': divergence ,
         'add_labels:list[str]':add_labels , 'sample_label:str':sample_label , 'alignment_label:str':alignment_label ,
         'bRemoveCurse:bool':bRemoveCurse , 'n_projections:int':n_projections , 'directory:str':directory , 'bQN:int':bQN ,
         'nNeighborFilter:list[int]':nNeighborFilter , 'heal_symmetry_break_method:str':heal_symmetry_break_method ,
         'epls_ownership:str':epls_ownership , 'bNonEuclideanBackprojection:bool':bNonEuclideanBackprojection ,
-        'Sfunc':Sfunc , 'bAddPies:bool':bAddPies }
+        'Sfunc':Sfunc , 'bAddPies:bool':bAddPies , 'bUseTDA':bUseTDA ,
+	'contraction_quantile:float': contraction_quantile , ' contraction_depth:float': contraction_depth }
             ofile = open ( header_str + runinfo_file , 'w' )
             for item in run_dict.items():
                 if 'list' in str(type(item[1])):
                     print ( item[0],'\t=\t [', ','.join([str(i) for i in item[1]]) ,']', file=ofile )
                 else :
                     print ( item[0],'\t=\t [', str(item[1]) ,']', file=ofile )
             print ( 'PYTHON GLOBALS:\n ',
@@ -224,15 +248,16 @@
     resdf_f , hierarch_f_df , soldf_f = create_mapping ( distm = distm_features ,
                      index_labels = adf.index.values , cmd = hierarchy_cmd , MF = MF_f ,
                      n_clusters  = n_clusters  , bExtreme = bExtreme ,
                      bUseUmap    = bUseUmap    , umap_dimension = umap_dimension,
                      n_neighbors = n_neighbors , local_connectivity = local_connectivity ,
                      transform_seed = transform_seed, n_proj = n_projections ,
                      bNonEuclideanBackprojection = bNonEuclideanBackprojection ,
-                     Sfunc = Sfunc )
+                     Sfunc = Sfunc , bUseTDA = bUseTDA ,
+                     contraction_quantile = contraction_quantile , contraction_depth=contraction_depth )
     if bVerbose :
         print ( 'FINISHED RESULTS > ', 'resdf_f.tsv , soldf_f.tsv , hierarch_f.tsv' )
     if not directory is None:
         resdf_f .index.name = header_str
         resdf_f .to_csv( header_str + 'resdf_f.tsv' , sep='\t' )
         soldf_f .to_csv( header_str + 'soldf_f.tsv' , sep='\t' )
         hierarch_f_df .to_csv( header_str + 'hierarch_f.tsv' , sep='\t' )
@@ -252,15 +277,16 @@
     resdf_s , hierarch_s_df , soldf_s = create_mapping ( distm = distm_samples ,
                      index_labels = adf.columns.values	, cmd = hierarchy_cmd , MF = MF_s ,
                      n_clusters   = n_clusters  	, bExtreme = bExtreme ,
                      bUseUmap     = bUseUmap    	, umap_dimension = umap_dimension,
                      n_neighbors  = n_neighbors 	, local_connectivity = local_connectivity ,
                      transform_seed = transform_seed	, n_proj = n_projections ,
                      bNonEuclideanBackprojection = bNonEuclideanBackprojection ,
-                     Sfunc = Sfunc )
+                     Sfunc = Sfunc , bUseTDA = bUseTDA ,
+                     contraction_quantile = contraction_quantile , contraction_depth=contraction_depth )
     #
     if bVerbose :
         print ( 'FINISHED RESULTS > ', 'resdf_s.tsv , soldf_s.tsv , hierarch_s.tsv' )
     if not directory is None :
         resdf_s .to_csv( header_str + 'resdf_s.tsv',sep='\t' )
         soldf_s .to_csv( header_str + 'soldf_s.tsv',sep='\t' )
         hierarch_s_df.to_csv( header_str + 'hierarch_s.tsv' , sep='\t' )
```

### Comparing `biocartograph-0.3.2/src/biocartograph/special.py` & `biocartograph-0.4.2/src/biocartograph/special.py`

 * *Files 23% similar despite different names*

```diff
@@ -50,21 +50,21 @@
         'in the following way :' ,
         'PAREN_GROUP_ID TAB CHILD_GROUP_ID','or:',
         'PROTF010\tPROTF001',
         ''
     ]
     print ( '\n'.join(desc__) )
 
-def read_rds_distance_matrix ( filename = '../res1/distance/distances.rds' ) :
+def read_rds_distance_matrix ( filename:str ) -> np.array :
     import rpy2.robjects as robjects
     from rpy2.robjects import pandas2ri
     from scipy.spatial.distance import pdist,squareform
     pandas2ri.activate()
     readRDS = robjects.r['readRDS']
-    return ( squareform(readRDS ('../res1/distance/distances.rds') ) )
+    return ( squareform(readRDS (filename) ) )
 
 def inplace_norm ( x:pd.DataFrame , n:int=10 , random_state:int=42 , axis:int=0 ) -> pd.DataFrame :
     from sklearn.preprocessing import quantile_transform
     x = x.T
     y = x.values[:-1]	# REMOVE GROUPING LABEL VALUES
     if axis == 0 :	# OVER ROWS
         nvals = quantile_transform (   y ,
@@ -121,14 +121,57 @@
         return ( pd.concat( [composition_df.T, fractions_df]).T )
     return ( composition_df )
 
 def pivot_data ( mdf:pd.DataFrame , index:str ='index' , column:str = 'sample', values:str = 'value' ) -> pd.DataFrame :
     pdf = mdf.pivot( index = index , columns = [column] , values = values )
     return ( pdf )
 
+def check_directory ( dir_string:str ,
+                      use_exclusion:str = 'pruned' ) -> list :
+    check_set  = {'tsv','csv','xlsx'}
+    if dir_string[-1] != '/':
+        dir_string += '/'
+    if not ( dir_string[0] == '~' or dir_string[0] == '/' ) :
+        print ( "INCLOMPLETE DIRECTORY" )
+    import os
+    contents = os.listdir(dir_string)
+    what = []
+    for thing in contents :
+        if 'str' in str(type(use_exclusion)):
+            if 'pruned' in thing :
+                continue
+        if thing.split('.')[-1] in check_set :
+            what.append( [dir_string+thing ,'\t' if '.tsv' in thing else ',' if '.csv' in thing else 'X' if '.xlsx' in thing else ' ' ] )
+    return ( what )
+
+def prune_dataframe( df:pd.DataFrame , indices:str , property_name:str , value_name:str ) -> pd.DataFrame :
+        from biocartograph.special import pivot_data
+        pdf = pivot_data( df, index = indices , column = property_name , values = value_name )
+        pdf = pdf.dropna( )
+        pdf = pdf.iloc[ np.inf != np.abs( 1.0/np.std(pdf.values,1) ) ,
+                        np.inf != np.abs( 1.0/np.std(pdf.values,0) ) ].copy().apply(pd.to_numeric)
+        pdf .loc[:,indices] = pdf.index
+        mdf = pdf.melt( id_vars = [indices] )
+        mdf = mdf.rename( columns = {'value':value_name} )
+        mdf = mdf.sort_values(by=[indices,property_name])
+        mdf .index = mdf.loc[:,indices]
+        mdf = mdf.loc[:,[property_name,value_name]]
+        return ( mdf )
+
+def create_file_lookup( files:list[str] ) -> dict :
+    file_lookup = dict()
+    for file in files :
+        with open(file[0],'r') as input :
+            for line in input :
+                columns = line.replace('\n','').split(file[1])
+                file_lookup[file[0]] = [ c for c in columns if len(c)>0 ]
+                break
+    return ( file_lookup )
+
+
 def reformat_results_to_gmtfile_pcfile (	header_str:str          = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' ,
 						hierarchy_file:str	= 'resdf_f.tsv' ,
 						hierarchy_id:str	= 'cids.user.'  ,
 						axis:int = 0, order:str = 'descending'  , bRedundant:bool=False ,
 						hierarchy_level_label:str = 'HCLN' , bErrorCheck:bool = False ) -> tuple[list] :
     #
     df = pd.read_csv( header_str+hierarchy_file , sep='\t' , index_col=0 )
@@ -225,12 +268,74 @@
 
     pc_of	= open ( header_str + hierarchy_file.split('.')[0] + '_pcfile.txt' , 'w' )
     print ( "parent\tchild" , file = pc_of )
     for g in PCL :
         print ( g[1]+'\t'+g[2], file = pc_of)
     pc_of.close()
 
+def rescreen (  header_str:str          = "../results/DMHMSY_Wed_Apr__5_10_02_33_2023_" ,
+                full_solution:str       = "hierarch_f.tsv" ,
+                o_filename:str          = None ) -> pd.DataFrame :
+    #
+    filename            = header_str + full_solution
+    #
+    df = pd.read_csv( filename , sep='\t', index_col=0 )
+    df.index = range(len(df))
+    #
+    from collections import Counter
+    L = len( df )
+    full_result_dict = dict()
+    for i in range( L ) :
+        arow = df.iloc[i,:].values
+        for item in Counter( list( Counter( arow ).values() ) ).items() :
+            if item[0] in full_result_dict :
+                full_result_dict[ item[0] ] += item[1]
+            else :
+                full_result_dict[ item[0] ]  = item[1]
+        print ( 'DONE' , i , 'OF' , L, 'OR',i/L )
+    df_ = pd.DataFrame( full_result_dict.items() , columns=['k','v'] )
+    if not o_filename is None :
+        df_.to_csv( o_filename , sep='\t' )
+    return ( df_ )
+
+def contraction ( value:float , q:float , d:float ) -> float :
+    if value <= 0 :
+        return ( 0.0 )
+    r   = value / q # wasteful slob ...
+    r2  = r*r
+    r4  = r2*r2
+    r6  = r4*r2
+    r12 = r6*r6
+    p   = ( 1/r12 - 1/r6 ) * d * (-1)
+    p   = 1. + 1. * (p<0) + p * (p>=0)
+    return ( value / p ) # WARNING ONLY FOR WASTEFUL SAIGAS
+
+def contract ( a:np.array , d:float=None , q:float=None , quantile:float=0.05 ) -> np.array :
+    nm = np.shape(a)
+    b  = a.reshape(-1)
+    d_,q_ = d,q
+    if d is None :
+        d_ = 1.0/list(set(sorted( b )))[1]
+    if q is None :
+        q_ = np.quantile( b , q=quantile )
+    # THIS OPERATION IS SLOW
+    P  = np.array(list(map( lambda x:contraction(x , q=q_ , d=d_) , b ))).reshape(nm)
+    return ( P )
+
+
+def contract_df ( a:pd.DataFrame , d:float=None , q:float=None , quantile:float=0.05 ) -> pd.DataFrame :
+    nm = np.shape(a.values)
+    b  = a.values.reshape(-1)
+    d_,q_ = d,q
+    if d is None :
+        d_ = 1.0/list(set(sorted( b )))[1]
+    if q is None :
+        q_ = np.quantile( b , q=quantile )
+    # THIS OPERATION IS SLOWER
+    return ( a.apply( lambda x : pd.Series([contraction(x_ , q=q_ , d=d_ ) for x_ in x],name=x.name,index=x.index) )  )
+
+
 if __name__ == '__main__':
     reformat_results_and_print_gmtfile_pcfile(header_str = '../results/DMHMSY_Fri_Mar_17_14_37_07_2023_' )
     reformat_results_and_print_gmtfile_pcfile(header_str = '../results/DMHMSY_Fri_Mar_17_16_00_47_2023_' )
```

