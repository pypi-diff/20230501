# Comparing `tmp/conversation_control-0.1.0.tar.gz` & `tmp/conversation_control-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conversation_control-0.1.0.tar", last modified: Fri Apr 28 14:39:07 2023, max compression
+gzip compressed data, was "conversation_control-0.1.2.tar", last modified: Mon May  1 21:14:31 2023, max compression
```

## Comparing `conversation_control-0.1.0.tar` & `conversation_control-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 zerpa     (1000) zerpa     (1000)        0 2023-04-28 14:39:07.534583 conversation_control-0.1.0/
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)     1087 2023-04-26 14:59:18.000000 conversation_control-0.1.0/LICENSE.txt
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)      362 2023-04-28 14:39:07.534583 conversation_control-0.1.0/PKG-INFO
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)        0 2023-04-28 12:48:48.000000 conversation_control-0.1.0/README.md
-drwxrwxr-x   0 zerpa     (1000) zerpa     (1000)        0 2023-04-28 14:39:07.533583 conversation_control-0.1.0/conversation_control/
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)     8185 2023-04-27 22:22:06.000000 conversation_control-0.1.0/conversation_control/__init__.py
-drwxrwxr-x   0 zerpa     (1000) zerpa     (1000)        0 2023-04-28 14:39:07.534583 conversation_control-0.1.0/conversation_control.egg-info/
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)      362 2023-04-28 14:39:07.000000 conversation_control-0.1.0/conversation_control.egg-info/PKG-INFO
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)      289 2023-04-28 14:39:07.000000 conversation_control-0.1.0/conversation_control.egg-info/SOURCES.txt
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)        1 2023-04-28 14:39:07.000000 conversation_control-0.1.0/conversation_control.egg-info/dependency_links.txt
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)       86 2023-04-28 14:29:12.000000 conversation_control-0.1.0/conversation_control.egg-info/pyproject
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)       21 2023-04-28 14:39:07.000000 conversation_control-0.1.0/conversation_control.egg-info/top_level.txt
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)       79 2023-04-28 14:39:07.535584 conversation_control-0.1.0/setup.cfg
--rw-rw-r--   0 zerpa     (1000) zerpa     (1000)      413 2023-04-28 14:28:27.000000 conversation_control-0.1.0/setup.py
+drwxrwxr-x   0 zerpa     (1000) zerpa     (1000)        0 2023-05-01 21:14:31.694084 conversation_control-0.1.2/
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)     1087 2023-04-26 14:59:18.000000 conversation_control-0.1.2/LICENSE.txt
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)      362 2023-05-01 21:14:31.694084 conversation_control-0.1.2/PKG-INFO
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)        0 2023-04-28 12:48:48.000000 conversation_control-0.1.2/README.md
+drwxrwxr-x   0 zerpa     (1000) zerpa     (1000)        0 2023-05-01 21:14:31.643082 conversation_control-0.1.2/conversation_control/
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)     8975 2023-05-01 20:24:02.000000 conversation_control-0.1.2/conversation_control/__init__.py
+drwxrwxr-x   0 zerpa     (1000) zerpa     (1000)        0 2023-05-01 21:14:31.694084 conversation_control-0.1.2/conversation_control.egg-info/
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)      362 2023-05-01 21:14:31.000000 conversation_control-0.1.2/conversation_control.egg-info/PKG-INFO
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)      289 2023-05-01 21:14:31.000000 conversation_control-0.1.2/conversation_control.egg-info/SOURCES.txt
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)        1 2023-05-01 21:14:31.000000 conversation_control-0.1.2/conversation_control.egg-info/dependency_links.txt
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)       86 2023-04-28 14:29:12.000000 conversation_control-0.1.2/conversation_control.egg-info/pyproject
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)       21 2023-05-01 21:14:31.000000 conversation_control-0.1.2/conversation_control.egg-info/top_level.txt
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)       79 2023-05-01 21:14:31.694084 conversation_control-0.1.2/setup.cfg
+-rw-rw-r--   0 zerpa     (1000) zerpa     (1000)      413 2023-05-01 21:12:57.000000 conversation_control-0.1.2/setup.py
```

### Comparing `conversation_control-0.1.0/LICENSE.txt` & `conversation_control-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `conversation_control-0.1.0/conversation_control/__init__.py` & `conversation_control-0.1.2/conversation_control/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import OrderedDict
 from langchain.chains import LLMChain,SequentialChain,ConversationChain
 from typing import Dict
-
+from dataclasses import asdict
 
 class ConversationState:
     def __init__(self,conversation):
         self.conversation=conversation
         self.last_response={}
         self.states=OrderedDict()
         self.current_state=None
@@ -28,37 +28,39 @@
         else:
             notbreak=True
         
         return output
 
 
 class ConversationControl:
-    def __init__(self,name,session,models,force_outputs=[]):
+    def __init__(self,name,session,models,force_outputs=[],bool_keys=["yes","no"]):
         self.name=name
         self.handlers={}
         self.checkers={}
         self.observation={}
         self.history=[]
         self.modelState=models["state"]
         self.modelStore=models["store"]
         self.modelEvent=models["event"]
         self.session=session
         self.max_intents=3
         self.force_outputs=[]
+        self.positive_positive,self.negative_key=bool_keys
         """
         states:{
             "id":"name",
             handlers:[],
             before_states[]
         }
         """
         with session() as sess:
             store=sess.query(self.modelStore).filter(
                 self.modelStore.name==name).first()
-            self.store=store.id
+            if store:
+                self.store=asdict(store)
         self.states={
         }
         self.global_handlers=[]
     def force(self,chain,inputs):
         intents=0
         while self.max_intents>intents:
             results=chain.generate(inputs)
@@ -73,28 +75,33 @@
 
     def prepare(self,fn):
         def wrapper(*args,**kwargs):
             self.chain=fn(*args,**kwargs)
             self.chain.control=self
         return wrapper
 
-    def process_handler(self,data):
-        event=self.get_event("is_bni_request")
+    def process_handler(self,name, data):
+        event=self.get_event(name)
         if event:
-            if not data["_is_bni_request"]:
+            if not self.observation[f"{name}"]:
                 if event["negative_response"]:
                     data["response"]=event["negative_response"]
                 if event["negative_result"]!=None:
-                    data["_is_bni_request@result"]=event["negative_result"]
+                    try:
+                        self.observation[f"{name}@result"]=json.loads(event["negative_result"])
+                    except:
+                        self.observation[f"{name}@result"]=None
             else:
                 if event["positive_response"]:
                     data["response"]=event["positive_response"]
                 if event["positive_result"]!=None:
-                    data["_is_bni_request@result"]=event["positive_result"]
-
+                    try:
+                        self.observation[f"{name}@result"]=json.loads(event["positive_result"])
+                    except :
+                        self.observation[f"{name}@result"]=None
 
 
 
     def handler_response(self,handler):
         self.global_handlers.append(handler)
     def add_state(self,state):
         if type(state)==state and "id" in state  and "handlers" in state and "before_states" in state:
@@ -104,14 +111,18 @@
     def add_handler(self,name):
         def wrapper(fn):
             """
             Ejecuta una accion manejando el estado de la conversacion
             """
             self.handlers[name]=fn
         return wrapper
+    def observe_bool(self,name,ctx):
+        self.observation[name]=False
+        if self.positive_key in ctx[name].lower():
+            self.observation[name]=True
     def check(self,name,callback):
         self.checkers[name]=callback
     def verify(self,output):
         handlers=[]
         for handler,checker in self.checkers.items():
             if checker(output):
                 handlers.append(handlers)
@@ -125,18 +136,19 @@
                 if before_states:
                     self.history.append(state_id)
 
 
     def get_event(self,name):
         from dataclasses import asdict
         with control.session() as sess:
-            instance=sess.query(control.modelEvent).filter(
-                control.modelEvent.store==self.store,
-                control.modelEvent.name==name).first()
-            return asdict(instance)
+            if self.store:
+                instance=sess.query(control.modelEvent).filter(
+                    control.modelEvent.store==self.store["id"],
+                    control.modelEvent.name==name).first()
+                return asdict(instance)
 
 
 
     def process(self,result):
         for handler in self.handlers:
             if handler in result:
                 self.handlers[handler](result,self.observation)
@@ -147,55 +159,57 @@
     def __call__(self):
         """
         Actualiza los handlers y states  en la base de datos
         ConversationState
         ConversationStore
         ConversationEvent
         """
-        print("PROCESANDO PARA CONTRUIR DB")
-        print(self.handlers)
-        print(self.states)
-        for handler in self.handlers:
-            with self.session() as sess:
-                #Verificamos los eventos y el store existan en la base de datos
-                results=sess.query(self.modelStore,self.modelEvent).filter(
-                    self.modelStore.name==self.name,
-                    self.modelEvent.handler==handler).join(self.modelEvent).first()
-                print("wwww",results)
-                if not results:
-                    store=self.modelStore(name=self.name)
-                    sess.add(store)
-                    sess.commit()
-                if not results:
-                    event=self.modelEvent(
-                        store=store.id,
-                        handler=handler)
-                    sess.add(event)
-                    sess.commit()
-
-        for state_name in self.states:
-            with self.session() as sess:
-                #Verificamos los states y el store existan en la base de datos
-                results=sess.query(
-                    self.modelStore,self.modelState).filter(
-                    self.modelStore.name==self.name,
-                    self.modelState.name==state_name).join(self.modelState).first()
-                #si el store no exite lo crea
-                if not results:
-                    store=self.modelStore(name=name)
-                    sess.add(store)
-                    sess.commit()
-                #si el state no existe lo crea
-                if not results:
-                    state=self.modelState(
-                        store=store.id,
-                        name=state_name)
-            
-                    sess.add(state)
-                    sess.commit()
+        with self.session() as sess:
+            for handler in self.handlers:
+                    #Verificamos los eventos y el store existan en la base de datos
+                    results=sess.query(self.modelStore,self.modelEvent).filter(
+                        self.modelStore.name==self.name,
+                        self.modelEvent.handler==handler).join(self.modelEvent).first()
+                    if results:
+                        store,event=results
+                    if not results:
+                        store=self.modelStore(
+                            name=self.name,
+                            assistant=self.name)
+                        sess.add(store)
+                        sess.commit()
+                    if not results:
+                        event=self.modelEvent(
+                            store=store.id,
+                            handler=handler)
+                        sess.add(event)
+                        sess.commit()
+
+            self.store=asdict(store)
+
+            for state_name in self.states:
+                
+                    #Verificamos los states y el store existan en la base de datos
+                    results=sess.query(
+                        self.modelStore,self.modelState).filter(
+                        self.modelStore.name==self.name,
+                        self.modelState.name==state_name).join(self.modelState).first()
+                    #si el store no exite lo crea
+                    if not results:
+                        store=self.modelStore(name=name)
+                        sess.add(store)
+                        sess.commit()
+                    #si el state no existe lo crea
+                    if not results:
+                        state=self.modelState(
+                            store=store.id,
+                            name=state_name)
+                
+                        sess.add(state)
+                        sess.commit()
 
 
 class SequentialChain(SequentialChain):
     control:ConversationControl=None
     def __init__(self,*args,**kwargs):
         super().__init__(*args,**kwargs)
```

