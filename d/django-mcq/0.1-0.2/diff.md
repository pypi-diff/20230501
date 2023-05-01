# Comparing `tmp/django-mcq-0.1.tar.gz` & `tmp/django-mcq-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-mcq-0.1.tar", last modified: Mon May  1 02:12:50 2023, max compression
+gzip compressed data, was "django-mcq-0.2.tar", last modified: Mon May  1 02:49:00 2023, max compression
```

## Comparing `django-mcq-0.1.tar` & `django-mcq-0.2.tar`

### file list

```diff
@@ -1,30 +1,52 @@
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:12:50.712564 django-mcq-0.1/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1063 2023-05-01 02:01:55.000000 django-mcq-0.1/LICENSE
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       63 2023-05-01 02:01:55.000000 django-mcq-0.1/MANIFEST.in
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1448 2023-05-01 02:12:50.712564 django-mcq-0.1/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      697 2023-05-01 02:06:03.000000 django-mcq-0.1/README.md
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:12:50.708563 django-mcq-0.1/django_mcq.egg-info/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1448 2023-05-01 02:12:50.000000 django-mcq-0.1/django_mcq.egg-info/PKG-INFO
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      492 2023-05-01 02:12:50.000000 django-mcq-0.1/django_mcq.egg-info/SOURCES.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-01 02:12:50.000000 django-mcq-0.1/django_mcq.egg-info/dependency_links.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-01 02:12:50.000000 django-mcq-0.1/django_mcq.egg-info/not-zip-safe
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       14 2023-05-01 02:12:50.000000 django-mcq-0.1/django_mcq.egg-info/requires.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        5 2023-05-01 02:12:50.000000 django-mcq-0.1/django_mcq.egg-info/top_level.txt
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      104 2023-05-01 02:01:55.000000 django-mcq-0.1/pyproject.toml
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:12:50.708563 django-mcq-0.1/quiz/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/__init__.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       63 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/admin.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      140 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/apps.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      879 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/forms.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:12:50.708563 django-mcq-0.1/quiz/migrations/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     6373 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/migrations/0001_initial.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/migrations/__init__.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     2655 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/models.py
-drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:12:50.712564 django-mcq-0.1/quiz/templatetags/
--rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/templatetags/__init__.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      995 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/templatetags/quiz_extras.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       60 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/tests.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)      646 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/urls.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     6923 2023-05-01 02:01:55.000000 django-mcq-0.1/quiz/views.py
--rw-rw-r--   0 suhail    (1000) suhail    (1000)       38 2023-05-01 02:12:50.712564 django-mcq-0.1/setup.cfg
--rw-rw-r--   0 suhail    (1000) suhail    (1000)     1078 2023-05-01 02:12:23.000000 django-mcq-0.1/setup.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.474079 django-mcq-0.2/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1063 2023-05-01 02:01:55.000000 django-mcq-0.2/LICENSE
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       61 2023-05-01 02:23:43.000000 django-mcq-0.2/MANIFEST.in
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-05-01 02:49:00.474079 django-mcq-0.2/PKG-INFO
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1044 2023-05-01 02:48:40.000000 django-mcq-0.2/README.md
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.462079 django-mcq-0.2/django_mcq.egg-info/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1795 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/PKG-INFO
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1110 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/SOURCES.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/dependency_links.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        1 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/not-zip-safe
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       14 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/requires.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        5 2023-05-01 02:49:00.000000 django-mcq-0.2/django_mcq.egg-info/top_level.txt
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      104 2023-05-01 02:01:55.000000 django-mcq-0.2/pyproject.toml
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.466079 django-mcq-0.2/quiz/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/__init__.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       63 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/admin.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      140 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/apps.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.466079 django-mcq-0.2/quiz/fixtures/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)    16766 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/fixtures/sample_quizzes.json
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      879 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/forms.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.466079 django-mcq-0.2/quiz/migrations/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     6373 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/migrations/0001_initial.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/migrations/__init__.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     2655 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/models.py
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.462079 django-mcq-0.2/quiz/static/
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.466079 django-mcq-0.2/quiz/static/datatables/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     5222 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/datatables/dataTables.bootstrap4.min.css
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     2085 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/datatables/dataTables.bootstrap4.min.js
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)    82411 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/datatables/jquery.dataTables.min.js
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.470079 django-mcq-0.2/quiz/static/quiz/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      533 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/quiz/app.css
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)   141997 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/quiz/bootstrap.min.css
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)    86927 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/static/quiz/jquery-3.3.1.min.js
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.462079 django-mcq-0.2/quiz/templates/
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.470079 django-mcq-0.2/quiz/templates/quiz/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      670 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/_header.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      801 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/base.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      384 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/interests_form.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1913 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/quiz_list.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1683 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/quiz_result.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1251 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/student_detail.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     2396 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/student_list.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      685 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/take_quiz_form.html
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      847 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templates/quiz/taken_quiz_list.html
+drwxrwxr-x   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:49:00.470079 django-mcq-0.2/quiz/templatetags/
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)        0 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templatetags/__init__.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      995 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/templatetags/quiz_extras.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       60 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/tests.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)      646 2023-05-01 02:01:55.000000 django-mcq-0.2/quiz/urls.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     6919 2023-05-01 02:38:06.000000 django-mcq-0.2/quiz/views.py
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)       38 2023-05-01 02:49:00.474079 django-mcq-0.2/setup.cfg
+-rw-rw-r--   0 suhail    (1000) suhail    (1000)     1078 2023-05-01 02:33:04.000000 django-mcq-0.2/setup.py
```

### Comparing `django-mcq-0.1/LICENSE` & `django-mcq-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-mcq-0.1/PKG-INFO` & `django-mcq-0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mcq
-Version: 0.1
+Version: 0.2
 Summary: A configurable quiz app for Django.
 Home-page: https://github.com/suhailvs/django-mcq
 Author: Suhail VS
 Author-email: suhailvs@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -55,8 +55,25 @@
         </head>
         <body>
             {% block quiz_body %}{% endblock %}
             {% block quiz_js %}{% endblock %}
         </body>
     </html>
 
-    
+Migrate database:
+
+    python manage.py migrate
+
+Load sample quizzes:
+
+    python manage.py loaddata sample_quizzes.json
+
+Now login a user and navigate to <http://127.0.0.1:8000/quiz/>
+
+
+Packaging pypi
+--------------
+
+* delete files in `dist` folder
+* increment the version number in your `setup.py` file
+* `$ python3 -m build`
+* `twine upload dist/*`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-mcq Version: 0.1 Summary: A configurable
+Metadata-Version: 2.1 Name: django-mcq Version: 0.2 Summary: A configurable
 quiz app for Django. Home-page: https://github.com/suhailvs/django-mcq Author:
 Suhail VS Author-email: suhailvs@gmail.com License: MIT License Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
@@ -11,7 +11,12 @@
 Choice Question Installation ------------ Install django-mcq Run `pip install
 django-mcq`. Add `'quiz'` to your `INSTALLED_APPS` setting. INSTALLED_APPS =
 ( ... 'quiz', ... ) Add the following to your projects `urls.py` file.
 urlpatterns = [ ... path('quiz/', include('quiz.urls')), ] Create a template
 `quiz_base.html` file in **templates** folder:
 {% block quiz_css %}{% endblock %}
 {% block quiz_body %}{% endblock %} {% block quiz_js %}{% endblock %}
+Migrate database: python manage.py migrate Load sample quizzes: python
+manage.py loaddata sample_quizzes.json Now login a user and navigate to
+127.0.0.1:8000/quiz/> Packaging pypi -------------- * delete files in `dist`
+folder * increment the version number in your `setup.py` file * `$ python3 -
+m build` * `twine upload dist/*`
```

### Comparing `django-mcq-0.1/django_mcq.egg-info/PKG-INFO` & `django-mcq-0.2/django_mcq.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-mcq
-Version: 0.1
+Version: 0.2
 Summary: A configurable quiz app for Django.
 Home-page: https://github.com/suhailvs/django-mcq
 Author: Suhail VS
 Author-email: suhailvs@gmail.com
 License: MIT License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -55,8 +55,25 @@
         </head>
         <body>
             {% block quiz_body %}{% endblock %}
             {% block quiz_js %}{% endblock %}
         </body>
     </html>
 
-    
+Migrate database:
+
+    python manage.py migrate
+
+Load sample quizzes:
+
+    python manage.py loaddata sample_quizzes.json
+
+Now login a user and navigate to <http://127.0.0.1:8000/quiz/>
+
+
+Packaging pypi
+--------------
+
+* delete files in `dist` folder
+* increment the version number in your `setup.py` file
+* `$ python3 -m build`
+* `twine upload dist/*`
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-mcq Version: 0.1 Summary: A configurable
+Metadata-Version: 2.1 Name: django-mcq Version: 0.2 Summary: A configurable
 quiz app for Django. Home-page: https://github.com/suhailvs/django-mcq Author:
 Suhail VS Author-email: suhailvs@gmail.com License: MIT License Classifier:
 Environment :: Web Environment Classifier: Framework :: Django Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Internet
@@ -11,7 +11,12 @@
 Choice Question Installation ------------ Install django-mcq Run `pip install
 django-mcq`. Add `'quiz'` to your `INSTALLED_APPS` setting. INSTALLED_APPS =
 ( ... 'quiz', ... ) Add the following to your projects `urls.py` file.
 urlpatterns = [ ... path('quiz/', include('quiz.urls')), ] Create a template
 `quiz_base.html` file in **templates** folder:
 {% block quiz_css %}{% endblock %}
 {% block quiz_body %}{% endblock %} {% block quiz_js %}{% endblock %}
+Migrate database: python manage.py migrate Load sample quizzes: python
+manage.py loaddata sample_quizzes.json Now login a user and navigate to
+127.0.0.1:8000/quiz/> Packaging pypi -------------- * delete files in `dist`
+folder * increment the version number in your `setup.py` file * `$ python3 -
+m build` * `twine upload dist/*`
```

### Comparing `django-mcq-0.1/quiz/forms.py` & `django-mcq-0.2/quiz/forms.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.1/quiz/migrations/0001_initial.py` & `django-mcq-0.2/quiz/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.1/quiz/models.py` & `django-mcq-0.2/quiz/models.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.1/quiz/templatetags/quiz_extras.py` & `django-mcq-0.2/quiz/templatetags/quiz_extras.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.1/quiz/urls.py` & `django-mcq-0.2/quiz/urls.py`

 * *Files identical despite different names*

### Comparing `django-mcq-0.1/quiz/views.py` & `django-mcq-0.2/quiz/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         'form': form,
         'progress': progress,
         'answered_questions': total_questions - total_unanswered_questions,
         'total_questions': total_questions
     })
 
 
-# @method_decorator([login_required], name='dispatch')
+@method_decorator([login_required], name='dispatch')
 class StudentList(ListView):
     # model = get_user_model()
     paginate_by = 36
     template_name = 'quiz/student_list.html'
     context_object_name = 'students'
 
     def get_queryset(self):
@@ -157,15 +157,15 @@
         if query:
             # queryset = queryset.annotate(
             #     full_name = Concat('first_name','last_name')
             # ).filter(full_name__icontains = query)
             queryset = queryset.filter(user__username__icontains = query)
         return queryset
 
-# @method_decorator([login_required], name='dispatch')
+@method_decorator([login_required], name='dispatch')
 class StudentDetail(View):
     """Show Details of a Student"""
     def get(self, request, **kwargs):
         student = Student.objects.get(user_id = kwargs['student'])
         subjects = student.taken_quizzes.all() \
             .values('quiz__subject__name','quiz__subject__color') \
             .annotate(score = Sum('score')) \
```

### Comparing `django-mcq-0.1/setup.py` & `django-mcq-0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 readme = open('README.md', encoding='utf-8')
 long_description = readme.read()
 
 
 setup(
     name='django-mcq',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A configurable quiz app for Django.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/suhailvs/django-mcq',
```

