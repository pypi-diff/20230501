# Comparing `tmp/AI-Summarizer-1.0.2.tar.gz` & `tmp/AI-Summarizer-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AI-Summarizer-1.0.2.tar", last modified: Fri Apr 14 16:56:36 2023, max compression
+gzip compressed data, was "AI-Summarizer-1.0.3.tar", last modified: Mon May  1 14:18:52 2023, max compression
```

## Comparing `AI-Summarizer-1.0.2.tar` & `AI-Summarizer-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 psps       (502) staff       (20)        0 2023-04-14 16:56:36.426209 AI-Summarizer-1.0.2/
-drwxr-xr-x   0 psps       (502) staff       (20)        0 2023-04-14 16:56:36.420966 AI-Summarizer-1.0.2/AI_Summarizer.egg-info/
--rw-r--r--   0 psps       (502) staff       (20)     3913 2023-04-14 16:56:36.000000 AI-Summarizer-1.0.2/AI_Summarizer.egg-info/PKG-INFO
--rw-r--r--   0 psps       (502) staff       (20)      262 2023-04-14 16:56:36.000000 AI-Summarizer-1.0.2/AI_Summarizer.egg-info/SOURCES.txt
--rw-r--r--   0 psps       (502) staff       (20)        1 2023-04-14 16:56:36.000000 AI-Summarizer-1.0.2/AI_Summarizer.egg-info/dependency_links.txt
--rw-r--r--   0 psps       (502) staff       (20)       40 2023-04-14 16:56:36.000000 AI-Summarizer-1.0.2/AI_Summarizer.egg-info/requires.txt
--rw-r--r--   0 psps       (502) staff       (20)       14 2023-04-14 16:56:36.000000 AI-Summarizer-1.0.2/AI_Summarizer.egg-info/top_level.txt
--rw-r--r--   0 psps       (502) staff       (20)     3913 2023-04-14 16:56:36.425413 AI-Summarizer-1.0.2/PKG-INFO
-drwxr-xr-x   0 psps       (502) staff       (20)        0 2023-04-14 16:56:36.424067 AI-Summarizer-1.0.2/ai_summarizer/
--rw-r--r--   0 psps       (502) staff       (20)      145 2023-04-14 16:26:45.000000 AI-Summarizer-1.0.2/ai_summarizer/__init__.py
--rw-r--r--   0 psps       (502) staff       (20)        0 2023-04-14 15:31:15.000000 AI-Summarizer-1.0.2/ai_summarizer/init.py
--rw-r--r--   0 psps       (502) staff       (20)     4855 2023-04-14 16:17:18.000000 AI-Summarizer-1.0.2/ai_summarizer/main.py
--rw-r--r--   0 psps       (502) staff       (20)       38 2023-04-14 16:56:36.426466 AI-Summarizer-1.0.2/setup.cfg
--rw-r--r--   0 psps       (502) staff       (20)     1628 2023-04-14 16:55:55.000000 AI-Summarizer-1.0.2/setup.py
+drwxr-xr-x   0 psps       (502) staff       (20)        0 2023-05-01 14:18:52.036468 AI-Summarizer-1.0.3/
+drwxr-xr-x   0 psps       (502) staff       (20)        0 2023-05-01 14:18:52.032200 AI-Summarizer-1.0.3/AI_Summarizer.egg-info/
+-rw-r--r--   0 psps       (502) staff       (20)     3913 2023-05-01 14:18:50.000000 AI-Summarizer-1.0.3/AI_Summarizer.egg-info/PKG-INFO
+-rw-r--r--   0 psps       (502) staff       (20)      262 2023-05-01 14:18:50.000000 AI-Summarizer-1.0.3/AI_Summarizer.egg-info/SOURCES.txt
+-rw-r--r--   0 psps       (502) staff       (20)        1 2023-05-01 14:18:50.000000 AI-Summarizer-1.0.3/AI_Summarizer.egg-info/dependency_links.txt
+-rw-r--r--   0 psps       (502) staff       (20)       40 2023-05-01 14:18:50.000000 AI-Summarizer-1.0.3/AI_Summarizer.egg-info/requires.txt
+-rw-r--r--   0 psps       (502) staff       (20)       14 2023-05-01 14:18:50.000000 AI-Summarizer-1.0.3/AI_Summarizer.egg-info/top_level.txt
+-rw-r--r--   0 psps       (502) staff       (20)     3913 2023-05-01 14:18:52.035746 AI-Summarizer-1.0.3/PKG-INFO
+drwxr-xr-x   0 psps       (502) staff       (20)        0 2023-05-01 14:18:52.034683 AI-Summarizer-1.0.3/ai_summarizer/
+-rw-r--r--   0 psps       (502) staff       (20)      145 2023-04-14 16:26:45.000000 AI-Summarizer-1.0.3/ai_summarizer/__init__.py
+-rw-r--r--   0 psps       (502) staff       (20)        0 2023-04-14 15:31:15.000000 AI-Summarizer-1.0.3/ai_summarizer/init.py
+-rw-r--r--   0 psps       (502) staff       (20)     4891 2023-05-01 14:10:18.000000 AI-Summarizer-1.0.3/ai_summarizer/main.py
+-rw-r--r--   0 psps       (502) staff       (20)       38 2023-05-01 14:18:52.036645 AI-Summarizer-1.0.3/setup.cfg
+-rw-r--r--   0 psps       (502) staff       (20)     1628 2023-05-01 14:17:47.000000 AI-Summarizer-1.0.3/setup.py
```

### Comparing `AI-Summarizer-1.0.2/AI_Summarizer.egg-info/PKG-INFO` & `AI-Summarizer-1.0.3/AI_Summarizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AI-Summarizer
-Version: 1.0.2
+Version: 1.0.3
 Summary: AI Summarizer is a Python package that uses OpenAI's GPT-3.5 to summarize any given text.
 Home-page: https://github.com/pietrosperoni/ai-summarizer
 Author: Pietro Speroni di Fenizio
 Author-email: aisummarizer@piespe.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AI-Summarizer-1.0.2/PKG-INFO` & `AI-Summarizer-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AI-Summarizer
-Version: 1.0.2
+Version: 1.0.3
 Summary: AI Summarizer is a Python package that uses OpenAI's GPT-3.5 to summarize any given text.
 Home-page: https://github.com/pietrosperoni/ai-summarizer
 Author: Pietro Speroni di Fenizio
 Author-email: aisummarizer@piespe.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `AI-Summarizer-1.0.2/ai_summarizer/main.py` & `AI-Summarizer-1.0.3/ai_summarizer/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     part_b=A[split_indices:]
     return part_a, part_b
 
 def _recursive_merge_summarises_new(summary_1: str, summary_2: str):
     result="\n# \n"+summary_1+"\n# \n"+summary_2
     return result
 
-def _recursive_summarize_text(text: str, filter: str = None, summary_length: int = 500,model="gpt-3.5-turbo"):
+def _recursive_summarize_text(text: str, filter: str = None, summary_length: int = 500,model="gpt-3.5-turbo",max_number_tokens=4096):
     if filter:
         prompt_content = f"""I need you to summarise some text which is part of a bigger document. 
             You should summarise the text by filtering out what does not follows this guidelines: 
             {filter}.
             
             The content is here:
             {text}
@@ -70,15 +70,15 @@
             
             Now create a summary. The result should not be longer than {summary_length} words. 
             Don't speak about the text, say directly what the text says.
             Also do not add conclusions or morals to the summary. Stick to the facts.
             Don't repeat yourself"""
         
     n_tokens=get_number_of_tokens(prompt_content,model=model)
-    if n_tokens>4096:
+    if n_tokens>max_number_tokens:
         text_1,text_2=split_text_logically(text)
         summary_1=_recursive_summarize_text(text_1, filter, summary_length=summary_length,model=model)
         summary_2=_recursive_summarize_text(text_2, filter, summary_length=summary_length,model=model)
         summary=_recursive_merge_summarises_new(summary_1, summary_2)
         return summary
     
     try:
```

### Comparing `AI-Summarizer-1.0.2/setup.py` & `AI-Summarizer-1.0.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 
 
 setup(
     name="AI-Summarizer",
-    version="1.0.2",
+    version="1.0.3",
     description="""AI Summarizer is a Python package that uses OpenAI's GPT-3.5 to summarize any given text.
     You can input some text describing what kind of information you are interested in. 
     When the text is too long it splits it logically into different sections, to make it simpler to summarise""",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/pietrosperoni/ai-summarizer",
     author="Pietro Speroni di Fenizio",
```

