# Comparing `tmp/canvasrobot-0.5.4.tar.gz` & `tmp/canvasrobot-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canvasrobot-0.5.4.tar", max compression
+gzip compressed data, was "canvasrobot-0.6.1.tar", max compression
```

## Comparing `canvasrobot-0.5.4.tar` & `canvasrobot-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      229 2023-01-05 13:29:04.133543 canvasrobot-0.5.4/README.md
--rw-r--r--   0        0        0      149 2023-02-24 18:31:12.907311 canvasrobot-0.5.4/canvasrobot/__init__.py
--rw-r--r--   0        0        0    72798 2023-02-24 18:31:12.919667 canvasrobot-0.5.4/canvasrobot/canvas_robot.py
--rw-r--r--   0        0        0    10421 2023-02-03 19:00:57.185292 canvasrobot-0.5.4/canvasrobot/canvas_robot_model.py
--rw-r--r--   0        0        0      253 2022-09-26 16:27:03.128683 canvasrobot-0.5.4/canvasrobot/entities/__init__.py
--rw-r--r--   0        0        0      614 2022-09-26 15:58:04.046429 canvasrobot-0.5.4/canvasrobot/entities/course.py
--rw-r--r--   0        0        0      706 2022-06-21 19:22:01.073940 canvasrobot-0.5.4/canvasrobot/entities/guest.py
--rw-r--r--   0        0        0     1174 2022-09-26 16:25:47.367671 canvasrobot-0.5.4/canvasrobot/entities/quiz.py
--rw-r--r--   0        0        0     2289 2022-06-21 19:21:38.582514 canvasrobot-0.5.4/canvasrobot/entities/user.py
--rw-r--r--   0        0        0      618 2023-02-24 18:31:46.106180 canvasrobot-0.5.4/pyproject.toml
--rw-r--r--   0        0        0     1108 1970-01-01 00:00:00.000000 canvasrobot-0.5.4/setup.py
--rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 canvasrobot-0.5.4/PKG-INFO
+-rw-r--r--   0        0        0      229 2023-01-05 13:29:04.133543 canvasrobot-0.6.1/README.md
+-rw-r--r--   0        0        0      338 2023-05-01 21:47:36.875391 canvasrobot-0.6.1/canvasrobot/__init__.py
+-rw-r--r--   0        0        0    65809 2023-05-01 21:38:40.606868 canvasrobot-0.6.1/canvasrobot/canvas_robot.py
+-rw-r--r--   0        0        0    10381 2023-03-30 08:46:30.991283 canvasrobot-0.6.1/canvasrobot/canvas_robot_model.py
+-rw-r--r--   0        0        0      402 2023-03-09 18:01:08.232782 canvasrobot-0.6.1/canvasrobot/entities/__init__.py
+-rw-r--r--   0        0        0     1099 2023-03-09 17:33:17.174768 canvasrobot-0.6.1/canvasrobot/entities/course.py
+-rw-r--r--   0        0        0      663 2023-03-09 17:33:17.175051 canvasrobot-0.6.1/canvasrobot/entities/guest.py
+-rw-r--r--   0        0        0     1017 2023-03-09 17:33:17.175104 canvasrobot-0.6.1/canvasrobot/entities/quiz.py
+-rw-r--r--   0        0        0     2182 2023-03-09 17:42:32.613135 canvasrobot-0.6.1/canvasrobot/entities/user.py
+-rw-r--r--   0        0        0      687 2023-05-01 21:47:36.871925 canvasrobot-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      998 1970-01-01 00:00:00.000000 canvasrobot-0.6.1/PKG-INFO
```

### Comparing `canvasrobot-0.5.4/canvasrobot/canvas_robot.py` & `canvasrobot-0.6.1/canvasrobot/canvas_robot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,86 +1,50 @@
-import sys
-from collections.abc import Callable
 import io
 import json
 import mimetypes
-import os
+import osstatus
 import re
 import time
 from collections import namedtuple
-from collections import deque
 from datetime import datetime
-import threading
 
 import attrs
-from attrs import define, field, asdict
+from attrs import define, asdict
 import canvasapi
 import requests
 import logging
 
 from rich.logging import RichHandler
 from rich.progress import track
 from canvasapi.course import Course
 from canvasapi.util import combine_kwargs
 from openpyxl.styles import NamedStyle, Font, PatternFill, Alignment
 from openpyxl.utils import get_column_letter
 from openpyxl.workbook import Workbook
 from openpyxl.worksheet.dimensions import ColumnDimension, DimensionHolder
 
-from .canvas_robot_model import AC_YEAR, NEXT_YEAR, ENROLLMENT_TYPES, STUDADMIN, \
-    EDUCATIONS, COMMUNITIES, LocalDAL, SHORTNAMES, CanvasConfig, EXAMINATION_FOLDER
-from .entities import User, EnrollDTO, SearchTextInCourseDTO, QuestionDTO
+from .canvas_robot_model import AC_YEAR, NEXT_YEAR, ENROLLMENT_TYPES, \
+    EDUCATIONS, COMMUNITIES, LocalDAL, CanvasConfig, EXAMINATION_FOLDER
+from .entities import User, QuestionDTO, CourseMetadata, Grade, ExaminationDTO, Stats
 
-logging.getLogger("canvasapi").setLevel(logging.WARNING)  # we don't need the info messages
+logging.getLogger("canvasapi").setLevel(logging.WARNING)
+# we don't need the info messages
 # from this library
 
 logging.basicConfig(
     level=logging.INFO,
     format="%(asctime)s [%(levelname)s] %(message)s",
-    # formatter="%(asctime)s %(levelname)s %(process)s %(thread)s %(funcName)s():%(lineno)d %(message)s"
     handlers=[
         logging.FileHandler("canvasrobot.log"),
         RichHandler()
         # logging.StreamHandler(sys.stdout)
     ]
 )
 
 
-def get_api_data(app_window=False):
-    """ ask for canvas username and api key, uses keyring to
-    store the values in a safe space
-    like /home/[your username]/.config/python_keyring
-    # on Windows: /Users/[your username]/...
-    """
-
-    key = keyring.get_password(NAMESPACE, ENTRY)
-    if key in (None, ""):
-        msg = "Enter your Canvas APi Key see 'Add a token' at https://community.canvaslms.com/docs/DOC-16041"
-        key = simpledialog.askstring("Input",
-                                     msg,
-                                     parent=app_window) if app_window \
-            else Prompt.ask(msg)
-        keyring.set_password(NAMESPACE, ENTRY, key)
-
-    url = keyring.get_password(NAMESPACE, URL)
-    if url in (None, ""):
-        msg = "Enter your Canvas URL (something like https://tilburguniversity.instructure.com)"
-        url = simpledialog.askstring("Input",
-                                     msg,
-                                     parent=app_window) if app_window \
-            else Prompt.ask(msg)
-        keyring.set_password(NAMESPACE, URL, url)
-
-    return url, key
-
-
-def reset_api_data(app_window=None):
-    for key in (URL, ENTRY):
-        keyring.delete_password(NAMESPACE, key)
-
 
 # noinspection PyProtectedMember
 def file_update(file, **kwargs):
     """
         Updates a file.
         :calls: `PUT /api/v1/files/:id \
         <https://canvas.instructure.com/doc/api/files.html#method.files.update>`_
@@ -103,27 +67,14 @@
 
 
 class DibsaRetrieveError(Error):
     """Raised when connection to Dibsa or retrieval failed"""
     pass
 
 
-@define
-class Grade:
-    stud_name: str
-    stud_id: str
-    final_score: float
-    final_grade: float
-
-@define
-class ExaminationDTO:
-    course_id: int
-    course_name: str
-    name:str
-
 
 @define
 class LabelType:
     label: str
     field_type: str
 
 
@@ -142,137 +93,46 @@
     time_zone: str
     locale: str
     # effective_locale str)
     # calendar str)
     # lti_user_id str)
 
 
-# noinspection PyCallingNonCallable,PyRedeclaration,PyTypeChecker
-# AnswerOptions = dict[str, int]  # answer_text, answer_weigth
-@define
-class Answer:
-    """canvas answer see for a complete list of (valid) fields
-    https://canvas.instructure.com/doc/api/quiz_questions.html
-    #:~:text=An%20Answer-,object,-looks%20like%3A
-    """
-    answer_html: str
-    answer_weight: int
-
-
-@define
-class QuestionDTO:
-    answers: list[Answer]
-    question_name: str = ""
-    question_type: str = 'multiple_choice_question'  # another option is 'essay question'
-    question_text: str = ''
-    points_possible: str = '1.0'
-    correct_comments: str = ''
-    incorrect_comments: str = ''
-    neutral_comments: str = ''
-    correct_comments_html: str = ''
-    incorrect_comments_html: str = ''
-    neutral_comments_html: str = ''
-
-@define
-class Stats:
-    quiz_ids: list[int] = []
-    question_ids: list[int] = []
-
-
-@define
-class CourseMetadata:
-    nr_modules: int
-    nr_module_items: int
-    nr_pages: int
-    nr_assignments: int
-    nr_quizzes: int
-    nr_files: int
-    assignments_summary: str
-    examinations_summary: str
-    examination_candidates: str
-    # nr_collaborations: int
-
-    # #ext_urls: int
-    # avr_len_assignments: int
-
-
-class UpdateDatabaseThread(threading.Thread):
-
-    def __init__(self, group=None, target=None, name=None,
-                 msg_queue=None, stop_list=None, single_course=None, max_number=None,
-                 kwargs=None, canvasrobot=None):
-        super().__init__(group=group, target=target,
-                         name=name)
-        self.exc = None
-        assert msg_queue, "needs msg_queue parameter"
-        assert canvasrobot, "needs canvasrobot instance"
-        if stop_list is None:
-            self.stop_list = STOP_LIST
-        self.single_course = single_course
-        self.max_number = max_number
-        self.aim = "all courses"
-        if single_course:
-            self.aim = f"single course ({single_course})"
-        if max_number:
-            self.aim = f"first {max_courses} courses"
-
-        self.q = msg_queue
-        self.kwargs = kwargs
-
-    def update_database(self):
-        try:
-            robot.update_database_from_canvas(single_course=self.single_course,
-                                              stop_list=self.stop_list,
-                                              max_number=self.max_number)
-        except sqlite3.OperationalError as exc:
-            # NOT working to catch the db-is-locked Operational error
-            showerror(title="database", message=f"DB problem {exc}")
-
-    def run(self):
-        self.exc = None
-        try:
-            self.update_database()
-        except BaseException as exc:
-            self.exc = exc
-
-    def join(self, timeout=None):
-        threading.Thread.join(self, timeout)
-        if self.exc:
-            raise self.exec
-
 
 # noinspection PyTypeChecker,PyUnresolvedReferences,PyCallingNonCallable
 class CanvasRobot(object):
     db: callable
-    from collections import deque
     TOT_WEIGHT: int = 100
     year: int = AC_YEAR
     def __init__(self, reset_api_keys=False, years_back = 0, msg_queue=None):
         self.year = AC_YEAR - years_back
         self.queue = msg_queue
         config = CanvasConfig(reset_api_keys=reset_api_keys)
         self.canvas = canvasapi.Canvas(config.url, config.api_key)
-        self.admin = self.canvas.get_account(config.admin_id) if config.admin_id else None
+        self.admin = self.canvas.get_account(config.admin_id) if config.admin_id \
+            else None
         db_path = os.path.join(os.getcwd(),'databases')
         if not os.path.exists(db_path):
             # Create a new directory because it does not exist
             os.makedirs(db_path)
         self.db = LocalDAL()
         self.teacher_ids = self.lookup_teachers_db()
         self.internal_id = None
         logging.info("Canvasrobot started")
         self.errors = []
         self.actions = []
 
     def add_to_queue(self, msg, value):
-        self.queue.put((msg,value))
+        if self.queue:
+            self.queue.put((msg,value))
     def lookup_teachers_db(self):
         db = self.db
         teachers = db((db.course2user.role == 'T') &
-                      (db.course2user.user == db.user.id)).select(db.user.user_id, distinct=True)
+                      (db.course2user.user == db.user.id)).select(db.user.user_id,
+                                                                  distinct=True)
         teacher_ids = [teacher.user_id for teacher in teachers]
         return teacher_ids
 
     # COURSES----------------------------------------
     def get_course(self, course_id: int):
         """"":returns canvas course by its id"""
         return self.canvas.get_course(course_id)
@@ -329,15 +189,15 @@
         profile = self.create_profile(user.get_profile())
         return user, profile
 
     def is_teacher_canvas(self, user):
         """":param user """
         role_teacher = ENROLLMENT_TYPES['teacher']
         # check if param: user is teacher in one of the TST courses
-        for course in self.tst.get_courses():
+        for course in self.admin.get_courses():
             enrollments = course.get_enrollments()
             for enrollment in enrollments:
                 if enrollment.role == role_teacher and enrollment.user == user:
                     return True
         return False
 
     def is_teacher_db(self, user):
@@ -400,28 +260,37 @@
                 examination_candidates.append(candidate)
             submissions_summary = ""
             submissions = assignment.get_submissions()
             try:
                 for idx, submission in enumerate(submissions, start=1):
                     if assignment.name in examination_names:
                         if submission.submission_type == "online_upload":
-                            submissions_summary += (f"({idx}. {submission.submission_type}) graded "
+
+                            originality_str = (f"{submission.has_originality_report}"
+                            if hasattr(submission, 'has_originality_report')
+                            else "no has_originality_report attribute!\n")
+                            submissions_summary += (f"({idx}. "
+                                                    f"{submission.submission_type}) "
+                                                    f"graded "
                                                     f"{submission.grade} at "
                                                     f"{submission.graded_at}. "
                                                     f"Checked for plagiarism: "
-                                                    f"{submission.has_originality_report if hasattr(submission,'has_originality_report') else 'no has_originality_report attribute!'}\n"
+                                                    f"{originality_str}\n"
                                                     )
                         else:
-                            submissions_summary+=(f"({idx}. {submission.submission_type}) graded "
+                            submissions_summary+=(f"({idx}. "
+                                                  f"{submission.submission_type}) "
+                                                  f"graded "
                                                   f"{submission.grade} at "
                                                   f"{submission.graded_at}\n")
             except BaseException as exc:
                 logging.exception(f"In Course:{course_id} {course.name} "
                                   f"Assignment {assignment.name} "
-                                  f"Submission nr {idx} type{submission.type} {exc}")
+                                  f"Submission nr {idx} "
+                                  f"type{submission.type} {exc}")
                 raise
 
 
             assignments_summary+=f"\n{submissions_summary}"
         nr_assignments = len(list(assignments))
         quizzes = course.get_quizzes()
         nr_quizzes = len(list(quizzes))
@@ -432,33 +301,35 @@
         examination_files = 0
         for file in files:
             folder = course.get_folder(file.folder_id)
             if f"/{EXAMINATION_FOLDER}" in folder.full_name:
                 examination_files+=1
                 examinations_summary+=f"\n{file.display_name}"
         if examination_files == 0:
-            examinations_summary += f"\nNo examination files in folder {EXAMINATION_FOLDER}"
+            examinations_summary += (f"\nNo examination files in "
+                                     f"folder {EXAMINATION_FOLDER}")
         else:
-            examinations_summary += f"\nTotal: {examination_files} examination files"
+            examinations_summary += (f"\nTotal: {examination_files} "
+                                     f"examination files")
         # was this working earlier 2.2.0 ?
         # try:
         #    collaborations = course.get_collaborations()
         #    list_of_cols = [c for c in collaborations]
         #    nr_collaborations = len(list_of_collaborations)
         # except TypeError:
         #    nr_collaborations = None
-        md = CourseMetadata(nr_modules,
-                            nr_module_items,
-                            nr_pages,
-                            nr_assignments,
-                            nr_quizzes,
-                            nr_files,
-                            assignments_summary,
-                            examinations_summary,
-                            examination_candidates
+        md = CourseMetadata(nr_modules=nr_modules,
+                            nr_module_items=nr_module_items,
+                            nr_pages=nr_pages,
+                            nr_assignments=nr_assignments,
+                            nr_quizzes=nr_quizzes,
+                            nr_files=nr_files,
+                            assignments_summary=assignments_summary,
+                            examinations_summary=examinations_summary,
+                            examination_candidates=examination_candidates
                             )
         # examination_candidates: collect to create a canonical list
         return md
 
     def enroll_in_course(self,
                          search: str,
                          course_id: int,
@@ -499,33 +370,31 @@
         def set_id_to_course_id(course):
             course.id = course.course_id
             return course
 
         if from_db:
             db = self.db
             courses = db(
-                (db.course.ac_year == self.year)).select(db.course.ALL)  # field id is db id
+                (db.course.ac_year == self.year)).select(db.course.ALL)
             # map(set_id_to_course_id, courses)
         else:
-            courses = self.tst.get_courses()
+            courses = self.admin.get_courses()
             courses = filter(cur_year_active, courses)
         # for index, c in enumerate(courses):
         #     print(index, c.name)
         return courses
 
     def get_course_using_osiris_id(self, osiris_id):
         """
         :returns first TST course with sisid starting with
-        osiris_id in current ac. year"""
-        for course in self.tst.get_courses():
-            # only consider course if current year
+        osiris_id in selected  year"""
+        for course in self.admin.get_courses():
+            # only consider course if selected year
             if str(course.sis_course_id)[:4] != str(self.year):
                 continue
-            # if not hasattr(course, "course_code") or course.course_code is None:
-            #     continue
             if course.course_code.startswith(osiris_id):
                 return course
 
     def get_course_id_using_osiris_id_from_db(self, osiris_id: str):
         db = self.db
         rows = db((db.course.course_code == osiris_id) &
                   (db.course.ac_year == self.year)).select(db.course.course_id)
@@ -537,15 +406,16 @@
         """
         :param search_name:
         :param email to search on email
         try search name as a login, then the email if supplied otherwise use
         """
         try:
             user = self.canvas.get_user(search_name, 'sis_login_id')
-        except (canvasapi.exceptions.Unauthorized, canvasapi.exceptions.ResourceDoesNotExist):
+        except (canvasapi.exceptions.Unauthorized,
+                canvasapi.exceptions.ResourceDoesNotExist):
             if not email:
                 # out of options
                 self.errors.append(f'Unable to lookup {search_name} '
                                    f'using email, parameter not provided')
                 return False
             try:
                 user = self.canvas.get_user(email, 'email')
@@ -593,27 +463,28 @@
         edu_ids = community_edu_ids[c_id]
         students_dibsa = []
         students_canvas = []
         for edu_id in edu_ids:
             try:
                 students_dibsa += self.get_students_dibsa(edu_id.upper())
             except DibsaRetrieveError as e:
-                logger.error(e)
+                logging.error(e)
                 raise
         for student in students_dibsa:
             username = student['username']
             user = self.search_user(username)
             if not user:
                 continue
             students_canvas.append(user)
 
         return students_canvas
 
     def get_community(self, c_id):
-        # c_id can be an education (each education has a community) or acskills (all educations)
+        # c_id can be an education (each education has a community)
+        # or acskills (all educations)
         # Decide: add pm-ma to BA?
         #         pm-ulo to ULO?
         #         pm-macs to MACS
         try:
             course = self.get_course(COMMUNITIES[c_id])
         except IndexError:
             return None, ["wrong c_id"]
@@ -631,15 +502,15 @@
         return
 
     def add_observer_to_education(self, user, edu_id, report_only=False):
         """ add user as an observer to all courses of an education"""
         # todo: select courses using membership of education using osiris ids
         print(user)
         # idea: filter course of an education using db
-        for course in self.tst.get_courses():
+        for course in self.admin.get_courses():
             # only insert/update course if current year
             if str(course.sis_course_id)[:4] != str(self.year):
                 continue
             observers = course.get_users(enrollment_type="observer")
             for observer in observers:
                 if not hasattr(observer, 'login_id'):
                     continue
@@ -649,15 +520,15 @@
         """ remove user as an observer from all TST courses"""
         removed = []
         try:
             user = self.canvas.get_user(username, 'sis_login_id')
         except canvasapi.exceptions.ResourceDoesNotExist:
             return f"User {username} not found in Canvas"
 
-        for course in self.tst.get_courses():
+        for course in self.admin.get_courses():
             # only get a course if current year
             if str(course.sis_course_id)[:4] != str(self.year):
                 continue
             enrollments = course.get_enrollments(type="ObserverEnrollment")
             # specifying user_id is not allowed
             for enrollment in enrollments:
                 if enrollment.user_id != user.id:
@@ -685,40 +556,43 @@
             logging.error("{} {} not found".format(e.message, path))
             raise
         else:
             reader = csv.reader(ofile, delimiter=';', quotechar='"')
             header = reader.next()
             logging.debug(header)
             # db(db.teacher.id > 0).delete()
-            db(db.course2teacher.id > 0).delete()  # refresh all course2teacher couplings
+            db(db.course2teacher.id > 0).delete()
+            # refresh all course2teacher couplings
             for row in reader:
                 logging.debug(row)
                 assert len(row) == 7, "Error {0} fields!".format(len(row))
                 teacher_names = row[2].replace(' (T)',
                                                '').replace(' (U)',
                                                            '').replace(' en ',
                                                                        ', ').split(', ')
                 # phases = row[4].split(', ')
                 course_id = db.course.update_or_insert(db.course.course_base == row[0],
-                                                       course_base=row[0],  # unique
+                                                       course_base=row[0],
                                                        name=row[1],
-                                                       teacher_names=row[2],  # redundant
+                                                       teacher_names=row[2],
                                                        ects=int(row[3]),
                                                        phase=row[4],
                                                        department=row[5],
                                                        memo=row[6])
                 if not course_id:  # must be there
-                    course_id = db(db.course.course_base == row[0]).select(db.course.id)[0].id
+                    course_id = db(db.course.course_base ==
+                                   row[0]).select(db.course.id)[0].id
                 else:
                     logging.info("course added")
                 for t_name in teacher_names:
                     teacher_id = db.teacher.update_or_insert(db.teacher.name == t_name,
                                                              name=t_name)
                     if not teacher_id:
-                        teacher_id = db(db.teacher.name == t_name).select(db.teacher.id)[0].id
+                        teacher_id = db(db.teacher.name ==
+                                        t_name).select(db.teacher.id)[0].id
                     db.course2teacher.insert(course=course_id,
                                              teacher=teacher_id)
 
             db.commit()
             ofile.close()
         return
 
@@ -731,15 +605,15 @@
         :param params: parameters to tune command
         """
         self.open()  # open canvas object
         try:
             url = self.base_url + (self.commands[command].format(params)
                                    if params else self.commands[command])
         except Exception:
-            raise NotImplementedError("error in command {0} or params {1}".format(command, params))
+            raise NotImplementedError(f"error in command {command} or params {params}")
         else:
             try:
                 self.browser.get(url)
             except Exception as e:
                 raise ValueError("self.browser.get uses url {} e:{}".format(url, e))
             return self.browser
 
@@ -765,64 +639,23 @@
         else:
             assert self.internal_id
         # we need the primary key
         try:
             bbcourse_id = db(db.bbcourse.bb_id ==
                              self.internal_id).select(db.bbcourse.id).first().id
         except AttributeError:
-            logging.info('course_id {0} not found in our database!'.format(self.internal_id))
+            logging.info(f'course_id {self.internal_id} not found in our database!')
             return -1
 
-        logging.info('updating users for course_id {0}'.format(bbcourse_id))
+        logging.info(f'updating users for course_id {bbcourse_id}')
         # show overview enrolled users
-        self.execute_command('enrolled_users', self.internal_id)  # assumes course selected
+        self.execute_command('enrolled_users', self.internal_id)
+        # assumes course is selected
         count = 0
         count_students = 0
-
-        #         roles = {"Teaching Assistant": "TA",
-        #                  "Instructor": "I",
-        #                  "Student": "S",
-        #                  "Guest": "G"}
-        # for tr in #PEOPLE self.browser.find_elements_by_
-        # xpath('//*[@id="listContainer_databody"]//tr'):  # all rows
-        #     username = ths[0].text
-        #     if 'preview' in username:
-        #         continue
-        #     logging.info('user {0} found'.format(username))
-        #     first_name, last_name, email, role =
-        #     (tds[2].text, tds[3].text, tds[4].text, tds[5].text)
-        #     # lookup role
-        #     try:
-        #         role = roles[role]
-        #     except IndexError:
-        #         logging.error("var roles incomplete '{}:...' missing".format(rol))
-        #     inserted_id = None
-        #     try:
-        #         inserted_id = db.bbuser.update_or_insert(db.bbuser.username == username,
-        #                                                  username=username,
-        #                                                  first_name=first_name,
-        #                                                  last_name=last_name,
-        #                                                  email=email)
-        #     except Exception as e:
-        #         logging.error("{0} error inserting user {1}".format(e, username))
-        #     else:
-        #         count += 1
-        #         if role == 'S':
-        #             count_students += 1
-        #     # lookup user_id if existing
-        #     bbuser_id = inserted_id if inserted_id \
-        #         else db(db.bbuser.username == username).select(db.bbuser.id).first().id
-        #
-        #     db.bbcourse2user.update_or_insert(((db.bbcourse2user.bbcourse == bbcourse_id) &
-        #                                        (db.bbcourse2user.bbuser == bbuser_id) &
-        #                                        (db.bbcourse2user.role == role)),
-        #                                       bbcourse=bbcourse_id,
-        #                                       bbuser=bbuser_id,
-        #                                       role=role)
-        #
         # connect user to this course in db
         db.commit()
 
         return count, count_students
 
     def get_courses_data(self):
         """ for all courses: get a matrix and labels coursename and other fields from db
@@ -893,30 +726,28 @@
                 break
             logging.info("{}/{}:{}".format(count + 1, len(courses), course.name))
             self.goto(course.bb_id)
             areas = self.get_areas()  # top level areas (menu buttons)
             logging.info("#{} areas#".format(len(areas)))
             for area in areas:
                 self.goto_area(area)  # select content area
-                bb_files = self.get_files_from_area(level=0, area_name=area.name)  # recursive
+                bb_files = self.get_files_from_area(level=0, area_name=area.name)
+                # above function is recursive
                 logging.info("{} files#".format(len(bb_files)))
                 # test_file_name = bb_files[0].fname
                 self.update_documents(bb_files)  # record data files in database
                 total_files += bb_files
-        return "{} courses scanned {} files found".format(len(courses), len(total_files))
+        return "{} courses scanned {} files found".format(len(courses),
+                                                          len(total_files))
 
     # the delegates ---
     # noinspection PyRedeclaration
     def make_enroll_file(self, courseid):
         self.db.make_enroll_file(courseid)
 
-    # noinspection PyRedeclaration
-    def import_courses(self, filename="vakken" + NEXT_YEAR):
-        self.db.import_courses(filename)
-
     def _check_bb(self, suffix=NEXT_YEAR):
         self.db.check_bb(suffix)
 
     def show_user(self, user_id):
         self.execute_command('showuser', user_id)
         time.sleep(120)
 
@@ -953,28 +784,29 @@
     def get_list_of_documents(self):
         """ get documents/attachments from db als a list
         """
         db = self.db
         suffix = '-{}-'.format(self.year)
         try:
             items = db((db.bbcourse.course_suffix.contains(suffix)) &
-                       (db.bbdocument.bbcourse_id == db.bbcourse.id)).select(db.bbdocument.ALL)
+                       (db.bbdocument.bbcourse_id ==
+                        db.bbcourse.id)).select(db.bbdocument.ALL)
         except Exception as e:
             logging.error("*{0} error in get_list_of_ documents() "
                           "while selecting documents*".format(e))
             return []
         else:
             return items
 
     # noinspection PyUnresolvedReferences
     def download_documents_localfs(self):
         db = self.db
         counters = namedtuple('Counters', ['total', 'ok', 'failed'])
         items = self.get_list_of_documents()
-        counters.total = len(files)
+        counters.total = len(items)
         counters.ok = 0
         counters.failed = 0
         for item in items:
             status = self.download_file(fname=item.name, url=item.url)
             if status == 200:
                 counters.ok += 1
             else:
@@ -985,15 +817,15 @@
 
     # noinspection PyUnresolvedReferences
     def transfer_files_to_server(self):
         """transfer all documents in the bbdocument table to the server"""
         db = self.db
         counters = namedtuple('Counters', ['total', 'ok', 'failed'])
         items = self.get_list_of_documents()
-        counters.total = len(files)
+        counters.total = len(items)
         counters.ok = 0
         counters.failed = 0
         for item in items:
             status = self.transfer_file_to_server(fname=item.name, url=item.url)
             if status == 200:
                 counters.ok += 1
             else:
@@ -1001,81 +833,99 @@
             db(db.bbdocument.id == item.id).update(http_status=status)
         db.commit()
         return counters
 
     def get_examinations_from_database(self, candidate=False):
         db = self.db
         # include the NULL values
-        qry = ((db.examination.id>0)&
-               (db.examination.candidate==candidate)) if candidate else (db.examination.id > 0)
+        qry = ((db.course.ac_year==self.year)&
+               (db.examination.course==db.course.course_id)& # join examination courses
+               (db.examination.candidate==
+                candidate)) if candidate else ((db.course.ac_year==self.year)&
+                                               (db.examination.course==db.course.course_id))
         records = db( qry ).select(db.examination.ALL)
         return records
     def get_courses_from_database(self,
                                   skip_courses_without_students=False,
+                                  add_list=None,
                                   qry=None,
                                   orderby=None,
                                   fields=None):
         db = self.db
         if skip_courses_without_students:
-            cur_qry = (db.course.nr_students>0)
+            cur_qry = (db.course.nr_students>0) &(db.course.ac_year==self.year)
         else:
-            cur_qry = (db.course.id>0)
+            cur_qry = (db.course.ac_year==self.year)
+
 
         if qry:
             cur_qry = cur_qry & qry
 
+
         fields = fields or db.course.ALL
         orderby=orderby or db.course.course_code
         records = db(cur_qry).select(db.course.ALL,
                                      orderby=orderby)
 
         return records
     def get_course_from_database(self,course_id):
         db = self.db
-        record = db(db.course.course_id==course_id).select(db.course.ALL).first()
+        record = db(db.course.course_id==
+                    course_id).select(db.course.ALL).first()
         return record
     def delete_course_from_database(self,course_id):
         db = self.db
         result = db(db.course.course_id==course_id).delete()
         db.commit()
         return result
 
     def update_record_db(self, search_field, search_id, table ,field, value):
+
         db = self.db
         ud_fields = {field: value}
         #row = db(db[table][search_field] == search_id).select()
         #row2 = db(db.course.course_id == search_id).select()
-        result = db(db[table][search_field] == search_id).update(**ud_fields)
+        db(db[table][search_field] == search_id).update(**ud_fields)
         db.commit()
 
     # noinspection PyUnusedLocal
-    def update_database_from_canvas(self, single_course=None, max_number=None, stop_list=None):
+    def update_database_from_canvas(self,
+                                    single_course=None,
+                                    single_course_osiris_id=None,
+                                    max_number=None,
+                                    stop_list=None):
         """
-            Using the canvasapi to read the list of TST courses and
+            Using the canvasapi to read the TST courses for the selected year
+            (or a single course using canvas cours_id or osiris id) and
             - record internal_id course_id, fname and instructors in the
             table course
             - put teacher details in table user
             - collects info about assignments in assignment_summary
             - collects info about examinations in examination_summary
             - reports new tentamination candidates
             :return number of added/updated rows
             """
 
         db = self.db
-        msg= f'open courselist for year {self.year} - {self.year+1}'
-        self.add_to_queue(msg,None)
+        msg= f'open course(s) for year {self.year} - {self.year+1}'
+        self.add_to_queue(msg, None)
         logging.info(msg)
         num_rows = 0
-        # tst = self.canvas.get_account(6)  # admin account
-        courses=[self.get_course(single_course),] if single_course else self.admin.get_courses()
+        if single_course_osiris_id:
+            courses= [self.get_course_using_osiris_id(single_course_osiris_id)]
+        elif single_course:
+            courses = [self.get_course(single_course)]
+        else:
+            courses = self.admin.get_courses()
+
         num_courses = len(list(courses))
         max_number = max_number or num_courses
 
         for idx,course in enumerate(courses):
-            self.add_to_queue(course.name, (idx,num_courses))
+            self.add_to_queue("<Progress>", (course.name,idx,num_courses))
 
             # only insert/update course if current year unless single_course
             if (str(course.sis_course_id)[:4] != str(self.year)
                     or course.name.endswith('conclude')) and not single_course:
                 continue
             if course.name in (stop_list or []):
                 continue
@@ -1087,45 +937,48 @@
             teachers = course.get_users(enrollment_type="teacher")
             teachers_ids = []
             for teacher in teachers:
                 if not hasattr(teacher, 'login_id'):
                     continue
                 # print(teacher.name)
                 first_name, last_name, prefix = self.parse_sortable_name(teacher)
-                inserted_id = db.user.update_or_insert(db.user.username == teacher.login_id,
+                inserted_id = db.user.update_or_insert(db.user.username ==
+                                                       teacher.login_id,
                                                        user_id=teacher.id,
                                                        name=teacher.name,
                                                        first_name=first_name,
                                                        prefix=prefix,
                                                        last_name=last_name,
                                                        username=teacher.login_id,
                                                        email=teacher.email,
                                                        role='T')
                 teachers_ids.append(inserted_id or
-                                    db(db.user.username == teacher.login_id).select().first().id)
+                                    db(db.user.username ==
+                                       teacher.login_id).select().first().id)
             try:
-                # skips teachers with non-accepted invites (they don't have a login attribute)
+                # skips teachers with non-accepted invites
+                # (they don't have a login attribute)
                 teacher_logins = [teacher.login_id for teacher in teachers
                                   if hasattr(teacher, 'login_id')]
                 teacher_names = [teacher.name for teacher in teachers
                                  if hasattr(teacher, 'login_id')]
             except AttributeError as e:
-                msg = f"skipped teacher of {course.name} [{course.id}]"
+                msg = (f"skipped teacher of {course.name} "
+                       f"[{course.id}] due to {e}")
                 logging.warning(msg)
-                # print(e, msg)
                 continue
             logging.info("instructors: {0}".format(teacher_logins))  # instructors
 
             inserted_id = None
             format_str = "%Y-%m-%dT%H:%M:%SZ"
             creation_date = datetime.strptime(course.created_at, format_str)
             course_id = None
             examinations = self.get_examinations_from_database(candidate=False)
-            canonical_examination_names = [row.name for row in examinations if (row.course==course.id
-                                                                                and not row.candidate)]
+            canonical_examination_names = [row.name for row in examinations
+                                           if (row.course==course.id and not row.candidate)]
             md = self.course_metadata(course.id, canonical_examination_names)
             try:
                 course_id = db.course.update_or_insert(db.course.course_id == course.id,
                                                        course_id=course.id,
                                                        # status=course.workflow_state,
                                                        course_code=course.course_code.split('-')[0],
                                                        sis_code=course.sis_course_id,
@@ -1140,23 +993,26 @@
                                                        nr_assignments=md.nr_assignments,
                                                        nr_quizzes=md.nr_quizzes,
                                                        assignments_summary= md.assignments_summary,
                                                        examinations_summary = md.examinations_summary,
                                                        teachers=teacher_logins,
                                                        teachers_names=teacher_names)
             except Exception as e:
-                logging.exception("{0} error inserting {1}".format(e, course))
+                err = f"{e} error inserting {course.name}"
+                self.add_to_queue("<InsertError>", err)
+                logging.exception(err)
                 raise
             if course_id:
                 db(db.course.id == inserted_id).update(status=2)
             else:
                 course_id = db(db.course.course_id == course.id).select().first().id
             for cand in md.examination_candidates:
                 # candidate is True if course_name in examination_list else False
-                db.examination.update_or_insert((db.examination.course == cand.course_id)&
+                db.examination.update_or_insert((db.examination.course ==
+                                                 cand.course_id)&
                                                  (db.examination.name == cand.name),
                                                  course=cand.course_id,
                                                  course_name=cand.course_name,
                                                  name=cand.name,
                                                 )
             for user_id in teachers_ids:
                 db.course2user.update_or_insert((db.course2user.course == course_id) &
@@ -1164,14 +1020,17 @@
                                                 course=course_id,
                                                 user=user_id,
                                                 role='T')
 
             db.commit()
             num_rows += 1
 
+        self.add_to_queue("<Done>",
+                          (f"Update db from Canvas "
+                           f"{single_course or max_number or 'All courses'}"))
         return num_rows
 
     def is_user_valid(self, userinfo):
         """"":param userinfo (dict or named tuple or Storage with attributes id, login_id)
              :returns True for invalid user, detail"""
         if type(userinfo) == dict:
             # import collections
@@ -1443,15 +1302,15 @@
         ws.append(["Vakbenamimg", "", course.name])
         ws.append(["Vakcode", "", course.course_code])
         ws.append(["Datum tentamen", "", "[in te vullen]"])
         ws.append([])
         ws.append(["Student", "SIS User ID", "Final Score", "Final Grade"])
         # data
         for row in grades:
-            ws.append(attr.astuple(row))
+            ws.append(attrs.astuple(row))
 
         # set width
         dim_holder = DimensionHolder(worksheet=ws)
         widths = [25, 12, 12, 12]
         for index, col in enumerate(range(ws.min_column, ws.max_column + 1)):
             dim_holder[get_column_letter(col)] = ColumnDimension(ws,
                                                                  min=col,
@@ -1504,15 +1363,15 @@
         quiz_question = quiz.create_question(question=asdict(question_dto))
         logging.debug(f"{quiz} now contains {quiz_question}")
         return quiz_question.id
         # return f"{quiz} now contains {quiz_question}", quiz_question.id
 
     def create_quizzes_from_data(self,
                                  course_id: int,
-                                 question_format="Vraag {}.",
+                                 question_format="Question {}.",
                                  data=None,
                                  gui_root=None,
                                  gui_queue=None
                                  ):
         """
         :param course_id: Canvas course_id: the quizzes are added to this course
         :param question_format: used to create the question name.
@@ -1554,53 +1413,14 @@
                 gui_root.event_generate('<<CreateQuizzes:Progress>>')
 
         if gui_root:
             gui_root.event_generate('<<CreateQuizzes:Done>>')
 
         return stats
 
-    def create_quizzes_from_document(self, filename: str,
-                                     course_id: int,
-                                     question_format="Vraag {}.",
-                                     check_num_questions=None,
-                                     adjust_fontsize=True,
-                                     testrun=False):
-        """
-        :param adjust_fontsize: if true change fontsize
-        :param testrun: if true: print don't create
-        :param check_num_questions:
-        :param filename: filename of the Word document (docx) to process
-        :param course_id: Canvas course_id: the quizzes are added to this course
-        :param question_format: used to create the question name.
-        They will be numbered. Should contain '{}' is placehiolder
-        starting with 1
-        :return:
-        """
-        if '{}' not in question_format:
-            print(f"parameter 'question_format(={question_format})' "
-                  f"should contain {{}} als placeholder")
-            return False
-        for quiz_name, questions in w2q.parse_document_d2p(filename,
-                                                           check_num_questions,
-                                                           normalize_fontsize=adjust_fontsize):
-
-            if testrun:
-                return
-
-            msg, quiz_id = self.create_quiz(course_id=course_id,
-                                            title=quiz_name,
-                                            quiz_type="practice_quiz")
-            for index, (question_text, answers) in enumerate(questions):
-                answers_asdict = [attrs.asdict(answer) for answer in answers]
-                question_dto = QuestionDTO(question_name=question_format.format(index + 1),
-                                           question_text=question_text,
-                                           answers=answers_asdict)
-                robot.create_question(course_id=COURSE_ID,
-                                      quiz_id=quiz_id,
-                                      question_dto=question_dto)
 
     def get_course_tab_by_label(self, course_id: int, label: str):
         course = self.get_course(course_id)
         for tab in course.get_tabs():
             if tab.label == label:
                 return tab
 
@@ -1608,35 +1428,37 @@
         course = self.get_course(course_id)
 
         foldernames = [f.full_name for f in course.get_folders()]
         if f"course files/{foldername}" in foldernames:
             logging.info(f"No action needed: Folder '(course) files/{foldername}' "
                          f"already in ({course_id})")
             return -1
-        folder_id = course.create_folder(foldername, parent_folder_path='/', locked=True)
+        folder_id = course.create_folder(foldername,
+                                         parent_folder_path='/',
+                                         locked=True)
         logging.info(f"Folder '(course) files/{foldername}' should be created now")
         return folder_id
 
     def create_folder_in_all_courses(self, foldername):
         for course in track(self.get_all_active_tst_courses(from_db=False),
                             description="All current courses..."):
-            folder_id = self.create_folder_in_course_files(course.id, foldername)
+            self.create_folder_in_course_files(course.id, foldername)
 
     def unpublish_subfolder_in_all_courses(self,
                                            foldername: str,
                                            files_too: bool = False,
                                            check_only: bool = False):
         for course in track(self.get_all_active_tst_courses(from_db=False),
                             description=(f"Checking all current"
                                          f" courses for folder '{foldername}'..." if check_only
                             else f"Unpublish all published folder {foldername}...")):
             if course.name.endswith("_conclude"):
                 continue
             # logging.info(course.name)
-            folder_id = self.unpublish_folderitems_in_course(course.id,
+            self.unpublish_folderitems_in_course(course.id,
                                                              foldername,
                                                              files_too,
                                                              check_only)
 
     def unpublish_folderitems_in_course(self, course_id: int,
                                         foldername: str,
                                         files_too: bool = False,
@@ -1684,15 +1506,15 @@
                     if files_tab.visibility == "public":
                         logging.warning(f"Files folder of {course.name}"
                                         f" ({course.id}) is visible")
                         # files_tab.visibility = "admins" # ! no change  without teachers approval!
                 except AttributeError:
                     logging.warning(f"Files tab visibility of {course.name} {course_id} missing")
 
-                folder_id = folder.id
+                # folder_id = folder.id
                 if not folder.locked:
                     if not check_only:
                         folder.update(locked=True)
                         folder_changes += 1
                         logging.info(
                             f"Folder '{foldername}' is now unpublished"
                             f" in course {course.name}")
```

### Comparing `canvasrobot-0.5.4/canvasrobot/canvas_robot_model.py` & `canvasrobot-0.6.1/canvasrobot/canvas_robot_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,23 @@
-from datetime import date, datetime, timedelta
+from datetime import datetime
 import os
 
 #try:
 #    from gluon import DAL, Field, XML, HTML
 #    from gluon.storage import Storage
 #except ImportError:
 from pydal import DAL, Field, validators
 import yaml
 import logging
 import logging.config
 
 from attrs import define
 import keyring
-import keyring.util.platform_ as keyring_platform
 # for UI use rich of tkinter
 from rich.prompt import Prompt
-from rich.console import Console
-import tkinter as tk
 from tkinter import simpledialog
 
 
 @define
 class CanvasConfig:
     """" save the urls and API_key in a save space using keyring"""
     namespace = "canvasrobot"
@@ -45,26 +42,25 @@
             self.reset_keys()
         self.get_values()
 
     def get_values(self):
         """ ask for canvas api key and url , uses keyring to
         store them in a safe space"""
 
-        values = dict()
         for field in self.api_fields:
             value = self.get_value(field["msg"], field["key"])
             self.__setattr__(field["key"], value)
 
     def get_value(self, msg, entry):
         value = keyring.get_password(self.namespace, entry)
         if value in (None, ""):
             value = simpledialog.askstring("Input",
                                            msg,
-                                           parent=app_window) if self.app_window \
-                else Prompt.ask(msg)
+                                           parent=self.app_window) \
+                if self.app_window else Prompt.ask(msg)
             keyring.set_password(self.namespace, entry, value)
             value = keyring.get_password(self.namespace, entry)
         return value
 
     def reset_keys(self):
         for field in self.api_fields:
             try:
@@ -198,26 +194,28 @@
                           Field('username', 'string'),
                           Field('fname', 'string'),
                           Field('first_name', 'string'),
                           Field('prefix', 'string'),
                           Field('last_name', 'string'),
                           Field('email', 'string'),
                           Field('primary_role', 'string', requires=valid_roles),
-                          format='%(first_name)s %(prefix)s %(last_name)s[%(username)s]',
+                          format=('%(first_name)s %(prefix)s '
+                                  '%(last_name)s[%(username)s]'),
                           singular='User',
                           plural='Users')
 
         self.define_table('course2user',
                           Field('course',
                                 'reference course',
                                 requires=validators.IS_IN_DB(self, 'course.id',
                                                              self.course._format)),
                           Field('user',
                                 'reference user',
-                                requires=validators.IS_IN_DB(self, 'user.id', self.user._format)),
+                                requires=validators.IS_IN_DB(self, 'user.id',
+                                                             self.user._format)),
                           Field('role', 'string',
                                 requires=valid_roles))
 
         # self.course.no_students = Field.Virtual('no_students',
         #                                       lambda row: self.((self.course2user.course == row.course.id) &
         #                                                         (self.course2user.role == 'S')).count())
```

### Comparing `canvasrobot-0.5.4/canvasrobot/entities/guest.py` & `canvasrobot-0.6.1/canvasrobot/entities/guest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import typing
-import collections
-import re
 import canvasapi
 
 
 class Guest:
     def __init__(self,
                  *args, **varg) -> None:
         if args and isinstance(args[0], canvasapi.user.User):
```

### Comparing `canvasrobot-0.5.4/canvasrobot/entities/user.py` & `canvasrobot-0.6.1/canvasrobot/entities/user.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import typing
 import collections
 import re
 import canvasapi
 
 class User:
     """Can be initialized with a canvasapi.user.User, a dict or with args & values"""
     def __init__(self,
@@ -34,20 +33,20 @@
         assert ", " in sortable_name, "sortable_name should contain comma"
         source = sortable_name
         pat = re.compile(
             r'(?P<last_name>[\w \-]+), (?P<first_name>\w+)\s?((\((?P<first_name_par>\w+)\))|'
             r'(\((?P<init>[\w.]+.)\)))?(\s*(?P<prefix>\w+))?')
         d = re.match(pat, source)
         if not d:
-            return res.ResponseFailure.create_exception_error("sortable_name failed parsing")
+            raise Exception("sortable_name failed parsing")
 
         self.first_name, self.prefix, self.last_name = (d['first_name_par'] or
                                                         d['first_name'], d['prefix'] or
                                                         '', d['last_name'])
-        return res.ResponseSuccess.create_default_success()
+
 
 
 
 # UserDTO = collections.namedtuple('UserDTO', 'user_id')
 # for now we can use User
 EnrollDTO = collections.namedtuple('EnrollDTO', 'user_id username course_id course role')
```

### Comparing `canvasrobot-0.5.4/pyproject.toml` & `canvasrobot-0.6.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "canvasrobot"
-version = "0.5.4"
+version = "0.6.1"
 description = "Library which uses Canvasapi https://canvasapi.readthedocs.io/en/stable/getting-started.html to provide a CanvasRobot class."
 authors = ["Nico de Groot <ndegroot0@gmail.com>",]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
 requests = "~=2.28.1"
@@ -17,11 +17,14 @@
 keyring = "*"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 mock = "*"
 pylint = "*"
+ruff = "*"
 #
+[tool.poetry_bumpversion.file."canvasrobot/__init__.py"]
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `canvasrobot-0.5.4/PKG-INFO` & `canvasrobot-0.6.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canvasrobot
-Version: 0.5.4
+Version: 0.6.1
 Summary: Library which uses Canvasapi https://canvasapi.readthedocs.io/en/stable/getting-started.html to provide a CanvasRobot class.
 Author: Nico de Groot
 Author-email: ndegroot0@gmail.com
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

