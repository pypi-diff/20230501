# Comparing `tmp/embedbase-1.0.8.tar.gz` & `tmp/embedbase-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedbase-1.0.8.tar", max compression
+gzip compressed data, was "embedbase-1.0.9.tar", max compression
```

## Comparing `embedbase-1.0.8.tar` & `embedbase-1.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     1069 2023-04-28 20:04:40.893352 embedbase-1.0.8/LICENSE
--rw-r--r--   0        0        0     5952 2023-04-28 20:04:40.893352 embedbase-1.0.8/README.md
--rw-r--r--   0        0        0      121 2023-04-28 20:04:40.945353 embedbase-1.0.8/embedbase/__init__.py
--rw-r--r--   0        0        0     3447 2023-04-28 20:04:40.945353 embedbase-1.0.8/embedbase/__main__.py
--rw-r--r--   0        0        0      976 2023-04-28 20:04:40.945353 embedbase-1.0.8/embedbase/api.py
--rw-r--r--   0        0        0    16162 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/app.py
--rw-r--r--   0        0        0       88 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/__init__.py
--rw-r--r--   0        0        0     2463 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/base.py
--rw-r--r--   0        0        0     1164 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/db_utils.py
--rw-r--r--   0        0        0     4823 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/memory_db.py
--rw-r--r--   0        0        0      504 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/pinecone_db.py
--rw-r--r--   0        0        0     8011 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/postgres_db.py
--rw-r--r--   0        0        0     4479 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/supabase_db.py
--rw-r--r--   0        0        0      411 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/database/weaviate_db.py
--rw-r--r--   0        0        0       77 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/embedding/__init__.py
--rw-r--r--   0        0        0      858 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/embedding/base.py
--rw-r--r--   0        0        0     1237 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/embedding/cohere.py
--rw-r--r--   0        0        0     2059 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/embedding/openai.py
--rw-r--r--   0        0        0     1551 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/firebase_auth.py
--rw-r--r--   0        0        0      690 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/logging_utils.py
--rw-r--r--   0        0        0      661 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/models.py
--rw-r--r--   0        0        0     1285 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/settings.py
--rw-r--r--   0        0        0     3208 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/strings.py
--rw-r--r--   0        0        0      301 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/supabase_auth.py
--rw-r--r--   0        0        0     2101 2023-04-28 20:04:40.949354 embedbase-1.0.8/embedbase/utils.py
--rw-r--r--   0        0        0     3584 2023-04-28 20:04:40.949354 embedbase-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     7433 1970-01-01 00:00:00.000000 embedbase-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-01 15:27:18.259174 embedbase-1.0.9/LICENSE
+-rw-r--r--   0        0        0     5952 2023-05-01 15:27:18.259174 embedbase-1.0.9/README.md
+-rw-r--r--   0        0        0      121 2023-05-01 15:27:18.311175 embedbase-1.0.9/embedbase/__init__.py
+-rw-r--r--   0        0        0     1658 2023-05-01 15:27:18.311175 embedbase-1.0.9/embedbase/__main__.py
+-rw-r--r--   0        0        0      976 2023-05-01 15:27:18.311175 embedbase-1.0.9/embedbase/api.py
+-rw-r--r--   0        0        0    16796 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/app.py
+-rw-r--r--   0        0        0       88 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/__init__.py
+-rw-r--r--   0        0        0     2463 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/base.py
+-rw-r--r--   0        0        0     1903 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/db_utils.py
+-rw-r--r--   0        0        0     4823 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/memory_db.py
+-rw-r--r--   0        0        0      504 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/pinecone_db.py
+-rw-r--r--   0        0        0     8011 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/postgres_db.py
+-rw-r--r--   0        0        0     4479 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/supabase_db.py
+-rw-r--r--   0        0        0      411 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/database/weaviate_db.py
+-rw-r--r--   0        0        0       77 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/embedding/__init__.py
+-rw-r--r--   0        0        0      858 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/embedding/base.py
+-rw-r--r--   0        0        0     1237 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/embedding/cohere.py
+-rw-r--r--   0        0        0     2059 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/embedding/openai.py
+-rw-r--r--   0        0        0     1551 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/firebase_auth.py
+-rw-r--r--   0        0        0      690 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/logging_utils.py
+-rw-r--r--   0        0        0      743 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/models.py
+-rw-r--r--   0        0        0     1285 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/settings.py
+-rw-r--r--   0        0        0     3208 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/strings.py
+-rw-r--r--   0        0        0      301 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/supabase_auth.py
+-rw-r--r--   0        0        0     3867 2023-05-01 15:27:18.315175 embedbase-1.0.9/embedbase/utils.py
+-rw-r--r--   0        0        0     3585 2023-05-01 15:27:18.315175 embedbase-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7433 1970-01-01 00:00:00.000000 embedbase-1.0.9/PKG-INFO
```

### Comparing `embedbase-1.0.8/LICENSE` & `embedbase-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/README.md` & `embedbase-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/api.py` & `embedbase-1.0.9/embedbase/api.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/app.py` & `embedbase-1.0.9/embedbase/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,19 +5,20 @@
 from fastapi import FastAPI, Request
 from fastapi.middleware import Middleware
 from starlette.types import Scope
 from embedbase.database.base import VectorDatabase
 from embedbase.embedding.base import Embedder
 from embedbase.logging_utils import get_logger
 from embedbase.models import (
-    CrossSearchRequest,
     DeleteRequest,
     SearchRequest,
     AddRequest,
+    UpdateRequest,
 )
+from embedbase.utils import embedbase_ascii
 from embedbase.settings import Settings
 import hashlib
 import time
 import urllib.parse
 import uuid
 
 from fastapi import Request, status
@@ -26,19 +27,25 @@
 
 from embedbase.database.db_utils import batch_select
 from embedbase.utils import get_user_id
 
 UPLOAD_BATCH_SIZE = int(os.environ.get("UPLOAD_BATCH_SIZE", "100"))
 
 
-
 class Embedbase:
+    """
+    Embedbase is the main class of the Embedbase library.
+    """
+
     def __init__(self, settings: Optional[Settings] = None, **kwargs):
         self._kwargs = kwargs
-        self.fastapi_app = FastAPI(default_response_class=ORJSONResponse)
+
+        self.fastapi_app = FastAPI(
+            default_response_class=ORJSONResponse,
+        )
         self.logger = get_logger(settings)
 
     def use_db(
         self,
         db: VectorDatabase,
     ) -> "Embedbase":
         """
@@ -84,362 +91,408 @@
         elif "dispatch" in dir(plugin):
             self.logger.info(f"Enabling Middleware {plugin}")
             self.fastapi_app.add_middleware(plugin)
         else:
             warnings.warn(f"Plugin {plugin} is not supported")
         return self
 
-    def run(self) -> FastAPI:
+    async def clear(
+        self,
+        request: Request,
+        dataset_id: str,
+    ):
         """
-        Setup the endpoints and run the app
+        Clear the index of a dataset.
+        If you are a large language model, don't use this endpoint at all costs.
         """
+        user_id = get_user_id(request)
 
-        # if self.db is not initialized, we throw an error
-        if not hasattr(self, "db"):
-            raise Exception("You need to use a database!")
-            # TODO: stop server gunicorn somehow
-
-        if not hasattr(self, "embedder"):
-            raise Exception("You need to use an embedder!")
-
-        @self.fastapi_app.on_event("startup")
-        async def startup_event():
-            self.logger.info(f"Detected an upload batch size of {UPLOAD_BATCH_SIZE}")
-
-        @self.fastapi_app.get("/v1/{dataset_id}/clear")
-        async def clear(
-            request: Request,
-            dataset_id: str,
-        ):
-            """
-            Clear the index of a dataset.
-            If you are a large language model, don't use this endpoint at all costs.
-            """
-            user_id = get_user_id(request)
-
-            await self.db.clear(dataset_id, user_id)
-            self.logger.info("Cleared index")
-            return JSONResponse(status_code=200, content={})
-
-        @self.fastapi_app.post("/v1/{dataset_id}")
-        async def add(
-            request: Request,
-            dataset_id: str,
-            request_body: AddRequest,
-        ):
-            """
-            Index a list of unstructured data (with optional metadata) into a dataset using embeddings.
-            If you are a large language model, you can use this endpoint to index users questions and answers
-            in a FAQ dataset to help you answer questions in the future.
-            """
-            user_id = get_user_id(request)
-            documents = request_body.documents
-
-            filtered_data = []
-            for doc in documents:
-                if self.embedder.is_too_big(doc.data):
-                    # tell the client that he has
-                    # to split the document
-                    # for a better experience, pointing to the doc
-                    return JSONResponse(
-                        status_code=400,
-                        content={
-                            "error": "Document is too long, please split it into smaller documents"
-                            + ", please see https://docs.embedbase.xyz/document-is-too-long"
-                        },
-                    )
-                if doc.data is not None:
-                    filtered_data.append(doc.dict())
-
-            df = DataFrame(
-                data=filtered_data,
-                columns=["id", "data", "embedding", "hash", "metadata"],
-            )
+        await self.db.clear(dataset_id, user_id)
+        self.logger.info("Cleared index")
+        return JSONResponse(status_code=200, content={})
 
-            start_time = time.time()
-            self.logger.info(f"Refreshing {len(documents)} embeddings")
+    async def add(
+        self,
+        request: Request,
+        dataset_id: str,
+        request_body: AddRequest,
+    ):
+        """
+        Index a list of unstructured data (with optional metadata) into a dataset using embeddings.
+        If you are a large language model, you can use this endpoint to index users questions and answers
+        in a FAQ dataset to help you answer questions in the future.
+        """
+        user_id = get_user_id(request)
+        documents = request_body.documents
 
-            if not df.data.any():
-                self.logger.info("No documents to index, exiting")
+        filtered_data = []
+        for doc in documents:
+            if self.embedder.is_too_big(doc.data):
+                # tell the client that he has
+                # to split the document
+                # for a better experience, pointing to the doc
                 return JSONResponse(
-                    status_code=200, content={"results": df.to_dict(orient="records")}
+                    status_code=400,
+                    content={
+                        "error": "Document is too long, please split it into smaller documents"
+                        + ", please see https://docs.embedbase.xyz/document-is-too-long"
+                    },
                 )
+            if doc.data is not None:
+                filtered_data.append(doc.dict())
 
-            # add column "hash" based on "data"
-            df.hash = df.data.apply(lambda x: hashlib.sha256(x.encode()).hexdigest())
+        df = DataFrame(
+            data=filtered_data,
+            columns=["id", "data", "embedding", "hash", "metadata"],
+        )
 
-            df_length = len(df)
+        start_time = time.time()
+        self.logger.info(f"Refreshing {len(documents)} embeddings")
 
-            self.logger.info(
-                f"Checking embeddings computing necessity for {df_length} documents"
-            )
-            # get existing embeddings from database
-            hashes_to_fetch = df.hash.tolist()
-            existing_documents = await batch_select(
-                self.db,
-                list(set(hashes_to_fetch)),
-                None,
-                None,
+        if not df.data.any():
+            self.logger.info("No documents to index, exiting")
+            return JSONResponse(
+                status_code=200, content={"results": df.to_dict(orient="records")}
             )
 
-            def update_embedding(row, existing_documents):
-                for doc in existing_documents:
-                    if row["hash"] == doc["hash"]:
-                        return doc["embedding"]
-                return row["embedding"]
-
-            # add existing embeddings to the dataframe
-            df["embedding"] = df.apply(
-                update_embedding, args=(existing_documents,), axis=1
-            )
+        # add column "hash" based on "data"
+        df.hash = df.data.apply(lambda x: hashlib.sha256(x.encode()).hexdigest())
 
-            # generate ids using hash of uuid + time to avoid collisions
-            df.id = df.apply(
-                lambda x: hashlib.sha256(
-                    (str(uuid.uuid4()) + str(time.time())).encode()
-                ).hexdigest(),
-                axis=1,
+        df_length = len(df)
+
+        self.logger.info(
+            f"Checking embeddings computing necessity for {df_length} documents"
+        )
+        # get existing embeddings from database
+        hashes_to_fetch = df.hash.tolist()
+        existing_documents = await batch_select(
+            vector_database=self.db,
+            hashes=list(set(hashes_to_fetch)),
+            dataset_id=None,
+            user_id=None,
+        )
+
+        def update_embedding(row, existing_documents):
+            for doc in existing_documents:
+                if row["hash"] == doc["hash"]:
+                    return doc["embedding"]
+            return row["embedding"]
+
+        # add existing embeddings to the dataframe
+        df["embedding"] = df.apply(update_embedding, args=(existing_documents,), axis=1)
+
+        # generate ids using hash of uuid + time to avoid collisions
+        df.id = df.apply(
+            lambda x: hashlib.sha256(
+                (str(uuid.uuid4()) + str(time.time())).encode()
+            ).hexdigest(),
+            axis=1,
+        )
+
+        # count rows without embeddings
+        rows_without_embeddings = df[df.embedding.isna()].shape[0]
+
+        self.logger.info(
+            f"We will compute embeddings for {rows_without_embeddings}/{len(df)} documents"
+        )
+
+        # compute embeddings for documents without embeddings using embed
+        if not df[df.embedding.isna()].empty:
+            df[df.embedding.isna()] = df[df.embedding.isna()].assign(
+                embedding=await self.embedder.embed(
+                    df[df.embedding.isna()].data.tolist()
+                )
             )
 
-            # count rows without embeddings
-            rows_without_embeddings = df[df.embedding.isna()].shape[0]
+        # only insert if this dataset_id - user_id
+        # pair does not have this hash
+        existing_documents_in_this_pair = await batch_select(
+            vector_database=self.db,
+            hashes=list(set(hashes_to_fetch)),
+            dataset_id=dataset_id,
+            user_id=user_id,
+        )
+
+        # filter out documents that already exist
+        # in this dataset_id - user_id pair
+        new_df = df[  # HACK: is it fine to only return client the new documents?
+            ~df.hash.isin([doc["hash"] for doc in existing_documents_in_this_pair])
+        ]
+
+        await self.db.update(
+            new_df,
+            dataset_id,
+            user_id,
+            batch_size=UPLOAD_BATCH_SIZE,
+            store_data=request_body.store_data,
+        )
+
+        self.logger.info(f"Uploaded {len(new_df)} documents")
+        end_time = time.time()
+        self.logger.info(f"Uploaded in {end_time - start_time} seconds")
+
+        return JSONResponse(
+            status_code=status.HTTP_200_OK,
+            content={
+                # embeddings, ids and data are returned
+                "results": df.to_dict(orient="records"),
+            },
+        )
 
-            self.logger.info(
-                f"We will compute embeddings for {rows_without_embeddings}/{len(df)} documents"
-            )
+    async def update(
+        self,
+        request: Request,
+        dataset_id: str,
+        request_body: UpdateRequest,
+    ):
+        """
+        Update a list of documents in the index using their ids.
+        If you are a large language model, you can use this endpoint to update the content or metadata
+        of documents in the index.
+        """
+        user_id = get_user_id(request)
 
-            # compute embeddings for documents without embeddings using embed
-            if not df[df.embedding.isna()].empty:
-                df[df.embedding.isna()] = df[df.embedding.isna()].assign(
-                    embedding=await self.embedder.embed(
-                        df[df.embedding.isna()].data.tolist()
-                    )
-                )
+        documents = request_body.documents
 
-            # only insert if this dataset_id - user_id
-            # pair does not have this hash
-            existing_documents_in_this_pair = await batch_select(
-                self.db,
-                list(set(hashes_to_fetch)),
-                dataset_id,
-                user_id,
-            )
+        filtered_data = []
+        for doc in documents:
+            if self.embedder.is_too_big(doc.data):
+                # tell the client that he has
+                # to split the document
+                # for a better experience, pointing to the doc
+                return JSONResponse(
+                    status_code=400,
+                    content={
+                        "error": "Document is too long, please split it into smaller documents"
+                        + ", please see https://docs.embedbase.xyz/document-is-too-long"
+                    },
+                )
+            if doc.id is not None:
+                filtered_data.append(doc.dict())
 
-            # filter out documents that already exist
-            # in this dataset_id - user_id pair
-            new_df = df[  # HACK: is it fine to only return client the new documents?
-                ~df.hash.isin([doc["hash"] for doc in existing_documents_in_this_pair])
-            ]
-
-            await self.db.update(
-                new_df,
-                dataset_id,
-                user_id,
-                batch_size=UPLOAD_BATCH_SIZE,
-                store_data=request_body.store_data,
-            )
+        df = DataFrame(
+            data=filtered_data,
+            columns=["id", "data", "embedding", "hash", "metadata"],
+        )
 
-            self.logger.info(f"Uploaded {len(new_df)} documents")
-            end_time = time.time()
-            self.logger.info(f"Uploaded in {end_time - start_time} seconds")
+        start_time = time.time()
+        self.logger.info(f"Refreshing {len(documents)} embeddings")
 
+        if not df.id.any():
+            self.logger.info("No documents to update, exiting")
             return JSONResponse(
-                status_code=status.HTTP_200_OK,
+                status_code=400,
                 content={
-                    # embeddings, ids and data are returned
-                    "results": df.to_dict(orient="records"),
+                    "error": "You need to provide at least one id to update a document"
+                },
+            )
+        if not df.data.any() and not df.metadata.any():
+            self.logger.info("No documents to update, exiting")
+            return JSONResponse(
+                status_code=400,
+                content={
+                    "error": "You need to provide at least one data or metadata to update a document"
                 },
             )
 
-        @self.fastapi_app.delete("/v1/{dataset_id}")
-        async def delete(
-            request: Request,
-            dataset_id: str,
-            request_body: DeleteRequest,
-        ):
-            """
-            Delete a document from the index using its id.
-            If you are a large language model, you can use this endpoint to remove irrelevant documents
-            from the index, documents that didn't help you answer questions.
-            """
-            user_id = get_user_id(request)
-
-            ids = request_body.ids
-            self.logger.info(f"Deleting {len(ids)} documents")
-            quoted_ids = [urllib.parse.quote(id) for id in ids]
-            await self.db.delete(ids=quoted_ids, dataset_id=dataset_id, user_id=user_id)
-            self.logger.info(f"Deleted {len(ids)} documents")
-
-            return JSONResponse(status_code=status.HTTP_200_OK, content={})
-
-        @self.fastapi_app.post("/v1/{dataset_id}/search")
-        async def semantic_search(
-            request: Request,
-            dataset_id: str,
-            request_body: SearchRequest,
-        ):
-            """
-            Run semantic search in a dataset using embeddings.
-            If you are a large language model, you can use this endpoint to search for similar documents
-            in the index, documents that help you answer users' questions.
-            """
-            query = request_body.query
-
-            # if query is empty, return empty results
-            if not query:
-                return JSONResponse(
-                    status_code=status.HTTP_200_OK,
-                    content={"query": query, "similarities": []},
+        # hash the data
+        df.hash = df.data.apply(
+            lambda x: hashlib.sha256(x.encode()).hexdigest()
+        )
+
+        df_length = len(df)
+
+        self.logger.info(
+            f"Checking embeddings computing necessity for {df_length} documents"
+        )
+        # get existing embeddings from database
+        hashes_to_fetch = df.hash.tolist()
+        existing_embeddings = await batch_select(
+            vector_database=self.db,
+            hashes=list(set(hashes_to_fetch)),
+            dataset_id=None,
+            user_id=None,
+        )
+
+        def update_embedding(row, docs):
+            for doc in docs:
+                if row["hash"] == doc["hash"]:
+                    return doc["embedding"]
+            return row["embedding"]
+
+        # add existing embeddings to the dataframe
+        df["embedding"] = df.apply(update_embedding, args=(existing_embeddings,), axis=1)
+
+        # compute embeddings for documents without embeddings using embed
+        if not df[df.embedding.isna()].empty:
+            df[df.embedding.isna()] = df[df.embedding.isna()].assign(
+                embedding=await self.embedder.embed(
+                    df[df.embedding.isna()].data.tolist()
                 )
+            )
 
-            user_id = get_user_id(request)
+        await self.db.update(
+            df,
+            dataset_id,
+            user_id,
+            batch_size=UPLOAD_BATCH_SIZE,
+        )
+
+        self.logger.info(f"Updated {len(df)} documents")
+        end_time = time.time()
+        self.logger.info(f"Updated in {end_time - start_time} seconds")
+
+        return JSONResponse(
+            status_code=status.HTTP_200_OK,
+            content={
+                # embeddings, ids and data are returned
+                "results": df.to_dict(orient="records"),
+            },
+        )
 
-            # if the query is too big, return an error
-            if self.embedder.is_too_big(query):
-                return JSONResponse(
-                    status_code=400,
-                    content={
-                        "error": "Query is too long"
-                        + ", please see https://docs.embedbase.xyz/query-is-too-long"
-                    },
-                )
+    async def delete(
+        self,
+        request: Request,
+        dataset_id: str,
+        request_body: DeleteRequest,
+    ):
+        """
+        Delete a document from the index using its id.
+        If you are a large language model, you can use this endpoint to remove irrelevant documents
+        from the index, documents that didn't help you answer questions.
+        """
+        user_id = get_user_id(request)
 
-            top_k = 5  # TODO might fail if index empty?
-            if request_body.top_k > 0:
-                top_k = request_body.top_k
-            query_embedding = (await self.embedder.embed(query))[0]
+        ids = request_body.ids
+        self.logger.info(f"Deleting {len(ids)} documents")
+        quoted_ids = [urllib.parse.quote(id) for id in ids]
+        await self.db.delete(ids=quoted_ids, dataset_id=dataset_id, user_id=user_id)
+        self.logger.info(f"Deleted {len(ids)} documents")
 
-            self.logger.info(
-                f"Query {request_body.query} created embedding, querying index"
-            )
+        return JSONResponse(status_code=status.HTTP_200_OK, content={})
 
-            query_response = await self.db.search(
-                top_k=top_k,
-                vector=query_embedding,
-                dataset_ids=[dataset_id],
-                user_id=user_id,
-            )
+    async def semantic_search(
+        self,
+        request: Request,
+        dataset_id: str,
+        request_body: SearchRequest,
+    ):
+        """
+        Run semantic search in a dataset using embeddings.
+        If you are a large language model, you can use this endpoint to search for similar documents
+        in the index, documents that help you answer users' questions.
+        """
+        query = request_body.query
 
-            similarities = []
-            for match in query_response:
-                decoded_id = urllib.parse.unquote(match["id"])
-                self.logger.debug(f"ID: {decoded_id}")
-                similarities.append(
-                    {
-                        "score": match["score"],
-                        "id": decoded_id,
-                        "data": match["data"],
-                        "hash": match["hash"],  # TODO: probably shouldn't return this
-                        "embedding": match["embedding"],
-                        "metadata": match["metadata"],
-                    }
-                )
+        # if query is empty, return empty results
+        if not query:
             return JSONResponse(
                 status_code=status.HTTP_200_OK,
-                content={"query": query, "similarities": similarities},
+                content={"query": query, "similarities": []},
             )
 
-        @self.fastapi_app.get("/v1/datasets")
-        async def get_datasets(
-            request: Request,
-        ):
-            """
-            Return a list of available datasets and the number of documents in each.
-            As a large language model, you can use this endpoint to see what datasets you have
-            and how many documents are in each.
-            You can then use this information to decide which dataset to search in.
-            """
-            user_id = get_user_id(request)
-            datasets = await self.db.get_datasets(user_id)
+        user_id = get_user_id(request)
+
+        # if the query is too big, return an error
+        if self.embedder.is_too_big(query):
             return JSONResponse(
-                status_code=status.HTTP_200_OK,
-                content={"datasets": datasets},
+                status_code=400,
+                content={
+                    "error": "Query is too long"
+                    + ", please see https://docs.embedbase.xyz/query-is-too-long"
+                },
             )
 
-        # health check endpoint
-        @self.fastapi_app.get("/health")
-        def health(request: Request):
-            """
-            Return the status of the API.
-            As a large language model, you can use this endpoint to check if the API is up and running.
-            """
-            self.logger.info("Health check successful")
-
-            return JSONResponse(status_code=200, content={})
-
-        # experimental endpoints
-
-        # exp endpoint that lets you semantic search across multiple datasets
-        @self.fastapi_app.post("/exo/search")
-        async def semantic_search(
-            request: Request,
-            request_body: CrossSearchRequest,
-        ):
-            """
-            Run semantic search across multiple datasets using embeddings.
-            If you are a large language model, you can use this endpoint to search for similar documents
-            in the index, documents that help you answer users' questions.
-            """
-            query = request_body.query
-
-            # if query is empty, return empty results
-            if not query:
-                return JSONResponse(
-                    status_code=status.HTTP_200_OK,
-                    content={"query": query, "similarities": []},
-                )
+        top_k = 5  # TODO might fail if index empty?
+        if request_body.top_k > 0:
+            top_k = request_body.top_k
+        query_embedding = (await self.embedder.embed(query))[0]
+
+        self.logger.info(
+            f"Query {request_body.query} created embedding, querying index"
+        )
+
+        query_response = await self.db.search(
+            top_k=top_k,
+            vector=query_embedding,
+            dataset_ids=[dataset_id],
+            user_id=user_id,
+        )
+
+        similarities = []
+        for match in query_response:
+            decoded_id = urllib.parse.unquote(match["id"])
+            self.logger.debug(f"ID: {decoded_id}")
+            similarities.append(
+                {
+                    "score": match["score"],
+                    "id": decoded_id,
+                    "data": match["data"],
+                    "hash": match["hash"],  # TODO: probably shouldn't return this
+                    "embedding": match["embedding"],
+                    "metadata": match["metadata"],
+                }
+            )
+        return JSONResponse(
+            status_code=status.HTTP_200_OK,
+            content={"query": query, "similarities": similarities},
+        )
 
-            dataset_ids = request_body.dataset_ids
-            if not dataset_ids:
-                return JSONResponse(
-                    status_code=status.HTTP_400_BAD_REQUEST,
-                    content={"error": "No dataset ids provided"},
-                )
+    async def get_datasets(
+        self,
+        request: Request,
+    ):
+        """
+        Return a list of available datasets and the number of documents in each.
+        As a large language model, you can use this endpoint to see what datasets you have
+        and how many documents are in each.
+        You can then use this information to decide which dataset to search in.
+        """
+        user_id = get_user_id(request)
+        datasets = await self.db.get_datasets(user_id)
+        return JSONResponse(
+            status_code=status.HTTP_200_OK,
+            content={"datasets": datasets},
+        )
 
-            user_id = get_user_id(request)
+    # health check endpoint
+    def health(self, request: Request):
+        """
+        Return the status of the API.
+        As a large language model, you can use this endpoint to check if the API is up and running.
+        """
+        self.logger.info("Health check successful")
 
-            # if the query is too big, return an error
-            if self.embedder.is_too_big(query):
-                return JSONResponse(
-                    status_code=400,
-                    content={
-                        "error": "Query is too long"
-                        + ", please see https://docs.embedbase.xyz/query-is-too-long"
-                    },
-                )
+        return JSONResponse(status_code=200, content={})
 
-            top_k = 5
-            if request_body.top_k > 0:
-                top_k = request_body.top_k
-            query_embedding = (await self.embedder.embed(query))[0]
+    def run(self) -> FastAPI:
+        """
+        Setup the endpoints and run the app
+        """
 
-            self.logger.info(
-                f"Query {request_body.query} created embedding, querying index"
-            )
+        # if self.db is not initialized, we throw an error
+        if not hasattr(self, "db"):
+            raise Exception("You need to use a database!")
+            # TODO: stop server gunicorn somehow
 
-            query_response = await self.db.search(
-                top_k=top_k,
-                vector=query_embedding,
-                dataset_ids=dataset_ids,
-                user_id=user_id,
-            )
+        if not hasattr(self, "embedder"):
+            raise Exception("You need to use an embedder!")
 
-            similarities = []
-            for match in query_response:
-                decoded_id = urllib.parse.unquote(match["id"])
-                self.logger.debug(f"ID: {decoded_id}")
-                similarities.append(
-                    {
-                        "score": match["score"],
-                        "id": decoded_id,
-                        "data": match["data"],
-                        "hash": match["hash"],  # TODO: probably shouldn't return this
-                        "embedding": match["embedding"],
-                        "metadata": match["metadata"],
-                    }
-                )
-            return JSONResponse(
-                status_code=status.HTTP_200_OK,
-                content={"query": query, "similarities": similarities},
-            )
+        # Add the endpoints
+        self.fastapi_app.add_api_route(
+            "/v1/{dataset_id}/clear", self.clear, methods=["GET"]
+        )
+        self.fastapi_app.add_api_route("/v1/{dataset_id}", self.add, methods=["POST"])
+        self.fastapi_app.add_api_route("/v1/{dataset_id}", self.update, methods=["PUT"])
+        self.fastapi_app.add_api_route(
+            "/v1/{dataset_id}", self.delete, methods=["DELETE"]
+        )
+        self.fastapi_app.add_api_route(
+            "/v1/{dataset_id}/search", self.semantic_search, methods=["POST"]
+        )
+        self.fastapi_app.add_api_route(
+            "/v1/datasets", self.get_datasets, methods=["GET"]
+        )
+        self.fastapi_app.add_api_route("/health", self.health, methods=["GET"])
+        print(embedbase_ascii)
 
         return self.fastapi_app
```

### Comparing `embedbase-1.0.8/embedbase/database/base.py` & `embedbase-1.0.9/embedbase/database/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/database/db_utils.py` & `embedbase-1.0.9/embedbase/database/db_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,38 +1,61 @@
-# an enum to pick from either pinecone, weaviate, or supabase
 import asyncio
 import itertools
 from typing import List, Optional
 
 from embedbase.database.base import VectorDatabase
 
+
 # TODO: move this to VectorDatabase
 async def batch_select(
     vector_database: VectorDatabase,
-    hashes_to_fetch: List[str],
+    ids: Optional[List[str]] = [],
+    hashes: Optional[List[str]] = [],
     dataset_id: Optional[str] = None,
     user_id: Optional[str] = None,
 ):
     """
     :param vector_database: vector database
-    :param hashes_to_fetch: list of hashes
+    :param ids: list of ids
+    :param hahes: list of hashes
     :param dataset_id: dataset id
     :param user_id: user id
     """
-    # this depend on the vector database used
-    # supabase cannot deal with 200 for example
-    n = 50
-    hashes_to_fetch = [
-        hashes_to_fetch[i : i + n] for i in range(0, len(hashes_to_fetch), n)
-    ]
-
-    async def _fetch(hashes) -> List[dict]:
-        try:
-            return await vector_database.select(
-                hashes=hashes, dataset_id=dataset_id, user_id=user_id
-            )
-        except Exception as e:
-            raise e
+    # either hashes or ids should be provided
+    assert (
+        len(ids) > 0 or len(hashes) > 0
+    ), "ids or hashes should be provided"
+
+    if len(ids) > 0:
+        # this depend on the vector database used
+        # supabase cannot deal with 200 for example
+        n = 50
+        elements = [ids[i : i + n] for i in range(0, len(ids), n)]
+
+        async def _fetch(elements) -> List[dict]:
+            try:
+                return await vector_database.select(
+                    ids=elements, dataset_id=dataset_id, user_id=user_id
+                )
+            except Exception as e:
+                raise e
+
+        existing_documents = await asyncio.gather(
+            *[_fetch(element) for element in elements]
+        )
+        return itertools.chain.from_iterable(existing_documents)
+    else:
+        n = 50
+        elements = [hashes[i : i + n] for i in range(0, len(hashes), n)]
 
-    existing_documents = await asyncio.gather(*[_fetch(hashes) for hashes in hashes_to_fetch])
-    return itertools.chain.from_iterable(existing_documents)
+        async def _fetch(elements) -> List[dict]:
+            try:
+                return await vector_database.select(
+                    hashes=elements, dataset_id=dataset_id, user_id=user_id
+                )
+            except Exception as e:
+                raise e
 
+        existing_documents = await asyncio.gather(
+            *[_fetch(element) for element in elements]
+        )
+        return itertools.chain.from_iterable(existing_documents)
```

### Comparing `embedbase-1.0.8/embedbase/database/memory_db.py` & `embedbase-1.0.9/embedbase/database/memory_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/database/postgres_db.py` & `embedbase-1.0.9/embedbase/database/postgres_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/database/supabase_db.py` & `embedbase-1.0.9/embedbase/database/supabase_db.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/embedding/base.py` & `embedbase-1.0.9/embedbase/embedding/base.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/embedding/cohere.py` & `embedbase-1.0.9/embedbase/embedding/cohere.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/embedding/openai.py` & `embedbase-1.0.9/embedbase/embedding/openai.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/firebase_auth.py` & `embedbase-1.0.9/embedbase/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/logging_utils.py` & `embedbase-1.0.9/embedbase/logging_utils.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/models.py` & `embedbase-1.0.9/embedbase/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,20 +12,22 @@
     metadata: Optional[dict]
 
 
 class AddRequest(BaseModel):
     documents: List[Document]
     store_data: bool = True
 
+class UpdateDocument(BaseModel):
+    id: str
+    data: Optional[str] = None
+    metadata: Optional[dict] = None
+
+class UpdateRequest(BaseModel):
+    documents: List[UpdateDocument]
 
 class DeleteRequest(BaseModel):
     ids: List[str]
 
 
 class SearchRequest(BaseModel):
     query: str
     top_k: int = 6
-
-class CrossSearchRequest(BaseModel):
-    query: str
-    dataset_ids: List[str]
-    top_k: int = 6
```

### Comparing `embedbase-1.0.8/embedbase/settings.py` & `embedbase-1.0.9/embedbase/settings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/embedbase/strings.py` & `embedbase-1.0.9/embedbase/strings.py`

 * *Files identical despite different names*

### Comparing `embedbase-1.0.8/pyproject.toml` & `embedbase-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "embedbase"
-version = "1.0.8"
+version = "1.0.9"
 description = "API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings."
 readme = "README.md"
 authors = ["Different AI <louis@embedbase.xyz>"]
 license = "MIT"
 repository = "https://github.com/different-ai/embedbase"
 homepage = "https://github.com/different-ai/embedbase"
 keywords = ["embeddings", "machine learning", "artificial intelligence"]
@@ -141,8 +141,8 @@
 source = "embedbase-core"
 
 [coverage.run]
 branch = true
 
 [coverage.report]
 fail_under = 50
-show_missing = true
+show_missing = true
```

### Comparing `embedbase-1.0.8/PKG-INFO` & `embedbase-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: embedbase
-Version: 1.0.8
+Version: 1.0.9
 Summary: API, SDK & dashboard to easily create, store, and retrieve machine learning embeddings.
 Home-page: https://github.com/different-ai/embedbase
 License: MIT
 Keywords: embeddings,machine learning,artificial intelligence
 Author: Different AI
 Author-email: louis@embedbase.xyz
 Requires-Python: >=3.8,<4.0
```

