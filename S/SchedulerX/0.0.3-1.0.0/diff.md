# Comparing `tmp/SchedulerX-0.0.3.tar.gz` & `tmp/SchedulerX-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SchedulerX-0.0.3.tar", last modified: Thu Mar  9 15:02:10 2023, max compression
+gzip compressed data, was "SchedulerX-1.0.0.tar", last modified: Sun Apr 30 21:02:40 2023, max compression
```

## Comparing `SchedulerX-0.0.3.tar` & `SchedulerX-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,19 @@
-drwxrwxr-x   0 khabir    (1000) khabir    (1000)        0 2023-03-09 15:02:10.026435 SchedulerX-0.0.3/
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     1073 2023-02-26 13:42:17.000000 SchedulerX-0.0.3/LICENSE
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     3825 2023-03-09 15:02:10.026435 SchedulerX-0.0.3/PKG-INFO
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     3299 2023-02-26 14:43:08.000000 SchedulerX-0.0.3/README.md
-drwxrwxr-x   0 khabir    (1000) khabir    (1000)        0 2023-03-09 15:02:10.022435 SchedulerX-0.0.3/SchedulerX.egg-info/
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     3825 2023-03-09 15:02:10.000000 SchedulerX-0.0.3/SchedulerX.egg-info/PKG-INFO
--rw-rw-r--   0 khabir    (1000) khabir    (1000)      451 2023-03-09 15:02:10.000000 SchedulerX-0.0.3/SchedulerX.egg-info/SOURCES.txt
--rw-rw-r--   0 khabir    (1000) khabir    (1000)        1 2023-03-09 15:02:10.000000 SchedulerX-0.0.3/SchedulerX.egg-info/dependency_links.txt
--rw-rw-r--   0 khabir    (1000) khabir    (1000)       11 2023-03-09 15:02:10.000000 SchedulerX-0.0.3/SchedulerX.egg-info/top_level.txt
--rw-rw-r--   0 khabir    (1000) khabir    (1000)      599 2023-03-09 14:59:17.000000 SchedulerX-0.0.3/pyproject.toml
-drwxrwxr-x   0 khabir    (1000) khabir    (1000)        0 2023-03-09 15:02:10.022435 SchedulerX-0.0.3/schedulerx/
--rw-rw-r--   0 khabir    (1000) khabir    (1000)      331 2023-03-09 14:59:19.000000 SchedulerX-0.0.3/schedulerx/__init__.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)      828 2023-03-09 14:59:25.000000 SchedulerX-0.0.3/schedulerx/config.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     3707 2023-02-26 10:56:07.000000 SchedulerX-0.0.3/schedulerx/file_manager.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)      236 2023-02-10 21:29:43.000000 SchedulerX-0.0.3/schedulerx/password_helper.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     1492 2023-02-26 10:51:43.000000 SchedulerX-0.0.3/schedulerx/permission_manager.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     2246 2023-02-26 11:29:42.000000 SchedulerX-0.0.3/schedulerx/run_command.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     1431 2023-03-09 14:59:29.000000 SchedulerX-0.0.3/schedulerx/service.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     1187 2023-02-26 11:03:45.000000 SchedulerX-0.0.3/schedulerx/service_timer_manager.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     1502 2023-02-26 10:51:43.000000 SchedulerX-0.0.3/schedulerx/simple_scheduler.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)     2397 2023-03-09 14:59:28.000000 SchedulerX-0.0.3/schedulerx/timer.py
--rw-rw-r--   0 khabir    (1000) khabir    (1000)       38 2023-03-09 15:02:10.026435 SchedulerX-0.0.3/setup.cfg
-drwxrwxr-x   0 khabir    (1000) khabir    (1000)        0 2023-03-09 15:02:10.026435 SchedulerX-0.0.3/tests/
--rw-rw-r--   0 khabir    (1000) khabir    (1000)      539 2023-03-09 14:45:26.000000 SchedulerX-0.0.3/tests/test.py
+drwxr-xr-x   0 khabir    (1000) khabir    (1000)        0 2023-04-30 21:02:40.513230 SchedulerX-1.0.0/
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)     1073 2023-02-26 13:42:17.000000 SchedulerX-1.0.0/LICENSE
+-rw-r--r--   0 khabir    (1000) khabir    (1000)     2670 2023-04-30 21:02:40.513230 SchedulerX-1.0.0/PKG-INFO
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)     2144 2023-04-30 20:38:35.000000 SchedulerX-1.0.0/README.md
+drwxr-xr-x   0 khabir    (1000) khabir    (1000)        0 2023-04-30 21:02:40.513230 SchedulerX-1.0.0/SchedulerX.egg-info/
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)     2670 2023-04-30 21:02:40.000000 SchedulerX-1.0.0/SchedulerX.egg-info/PKG-INFO
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)      300 2023-04-30 21:02:40.000000 SchedulerX-1.0.0/SchedulerX.egg-info/SOURCES.txt
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)        1 2023-04-30 21:02:40.000000 SchedulerX-1.0.0/SchedulerX.egg-info/dependency_links.txt
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)       11 2023-04-30 21:02:40.000000 SchedulerX-1.0.0/SchedulerX.egg-info/top_level.txt
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)      600 2023-04-30 21:01:51.000000 SchedulerX-1.0.0/pyproject.toml
+drwxr-xr-x   0 khabir    (1000) khabir    (1000)        0 2023-04-30 21:02:40.513230 SchedulerX-1.0.0/schedulerx/
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)      201 2023-04-30 20:57:46.000000 SchedulerX-1.0.0/schedulerx/__init__.py
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)      866 2023-04-30 20:50:14.000000 SchedulerX-1.0.0/schedulerx/file_manager.py
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)      503 2023-04-30 20:38:58.000000 SchedulerX-1.0.0/schedulerx/run_command.py
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)      967 2023-04-30 20:50:30.000000 SchedulerX-1.0.0/schedulerx/service.py
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)     1932 2023-04-30 20:52:39.000000 SchedulerX-1.0.0/schedulerx/timer.py
+-rw-r--r--   0 khabir    (1000) khabir    (1000)       38 2023-04-30 21:02:40.513230 SchedulerX-1.0.0/setup.cfg
+drwxr-xr-x   0 khabir    (1000) khabir    (1000)        0 2023-04-30 21:02:40.513230 SchedulerX-1.0.0/tests/
+-rw-rw-r--   0 khabir    (1000) khabir    (1000)      539 2023-03-09 14:45:26.000000 SchedulerX-1.0.0/tests/test.py
```

### Comparing `SchedulerX-0.0.3/LICENSE` & `SchedulerX-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SchedulerX-0.0.3/README.md` & `SchedulerX-1.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,142 +2,96 @@
 
 ## Authors
 
 - [@hakkm](https://www.github.com/hakkm)
 
 ## Installation
 
-```pip install SchedulerX```
+```pip install schedulerx```
 
-### Setting ROOT_PASSWORD to env variable 
-
-Handling systemd needs root privilege so this why we export it. so, you need to run this command and change the `<your-root-password>` with your root password
-
-```export ROOT_PASSWORD="<your-root-password>"```
-
-## Usage/Examples
-
-For simple usage, you have to know how to set [onCalendar in systemd](https://wiki.archlinux.org/title/systemd/Timers)
-
-```python3
-from schedulerx import SimpleScheduler
-
-scheduler = SimpleScheduler(
-    title="shutdown at midnight",
-    command="shutdown now",
-    on_calendar=@daily
-)
-
-scheduler.schedule()
-```
-
-for more complex usage you have to know about how we create a timer and a service in systemd  
-And then you can use ServiceTimerManager
-
-```python3
-from schedulerx import ServiceTimerManager
-
-service_timer = ServiceTimerManager(
-    service_filename="shutdown.service",
-    service_description="shutdown at midnight",
-    command="shutdown now",
-    timer_filename="shutdown.timer",
-    timer_description="shutdown at midnight timer",
-    on_calendar="@daily",
-)
-
-service_timer.schedule()
-```
+<!-- ## Usage/Examples -->
+<!---->
+<!-- For simple usage, you have to know how to set [onCalendar in systemd](https://wiki.archlinux.org/title/systemd/Timers) -->
+<!---->
+<!-- ```python3 -->
+<!-- from schedulerx import SimpleScheduler -->
+<!---->
+<!-- scheduler = SimpleScheduler( -->
+<!--     title="shutdown at midnight", -->
+<!--     command="shutdown now", -->
+<!--     on_calendar=@daily -->
+<!-- ) -->
+<!---->
+<!-- scheduler.schedule() -->
+<!-- ``` -->
+
+<!-- for more complex usage you have to know about how we create a timer and a service in systemd   -->
+<!-- And then you can use ServiceTimerManager -->
+<!---->
+<!-- ```python3 -->
+<!-- from schedulerx import ServiceTimerManager -->
+<!---->
+<!-- service_timer = ServiceTimerManager( -->
+<!--     service_filename="shutdown.service", -->
+<!--     service_description="shutdown at midnight", -->
+<!--     command="shutdown now", -->
+<!--     timer_filename="shutdown.timer", -->
+<!--     timer_description="shutdown at midnight timer", -->
+<!--     on_calendar="@daily", -->
+<!-- ) -->
+<!---->
+<!-- service_timer.schedule() -->
+<!-- ``` -->
 
 ## License
 
 [MIT](https://choosealicense.com/licenses/mit/)
 
 
 
 ## Class Diagram of SchedulerX
 
 ```mermaid
 classDiagram
 
-class PasswordHelper{
-    +get_root_password()
-}
 
 class CommandHandler{
-    +run_shell_command_with_input(command: string, password: string): string
-    +run_shell_command_as_root(command: string)
+    +run_shell_command(command: string): string
 }
 
-class PermissionManager{
-    -command_handler: CommandHandler
-    +change_path_permissions(path: string, permissions: string)
-    +is_writable(path: string): boolean
-}
 
 class FileManager{
     filename: string
-    overwrite: string = False
-    -permission_manager: PermissionManager
     <<property>> +file_full_path(): string
-    -save_origin_systemd_writable_permission()
     +create_file(content: string)
-    +is_file_exist(): boolean
-    +check_permissions()
 }
 
 class ServiceManager{
     +filename: string
     +command: string
     +description: string = ""
-    +overwrite: boolean = False
     +create_service_file()
     -get_service_text(): string
 }
 
 class TimerManager{
     +filename: string
     +description: string = ""
     +on_calendar: string
     +service_manager: ServiceManager
     -file_manager: FileManager
     -command_handler: CommandHandler
     -get_timer_text(): string
     +create_timer()
     +start_timer()
+    +enable_timer()
 }
 
-class ServiceTimerManager{
-    +service_filename: string
-    +service_description: string = ""
-    +command: string
-
-    +timer_filename: string
-    +timer_description: string = ""
-    +on_calendar: string
-    +overwrite: boolean = False
-    -service_manager: ServiceManager
-    -timer_manager: TimerManager
-    +schedule()
-    -create_service()
-    -create_timer()
-}
 
-class SimpleSchedule{
-    +title: string
-    +command: string
-    +on_calendar: string
-    +overwrite: boolean = False
-    +schedule()
-}
-CommandHandler --> PasswordHelper
-PermissionManager --> CommandHandler
-FileManager --> PermissionManager
+FileManager --> CommandHandler
 ServiceManager --> FileManager
 TimerManager --> ServiceManager
 TimerManager --> FileManager
 TimerManager --> CommandHandler
-ServiceTimerManager --> ServiceManager
-ServiceTimerManager --> TimerManager
-SimpleSchedule --> ServiceTimerManager
+
 
 ```
```

### Comparing `SchedulerX-0.0.3/pyproject.toml` & `SchedulerX-1.0.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "SchedulerX"
-version = "0.0.3"
+version = "1.0.0"
 authors = [
   { name="Khabir Abdelhakim", email="hakim1khabir2@gmail.com" },
 ]
 description = "Schedule a task using systemd services and timer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: Unix",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hakkm/service-timer"
-"Bug Tracker" = "https://github.com/hakkm/service-timer/issues"
+"Bug Tracker" = "https://github.com/hakkm/service-timer/issues"
```

### Comparing `SchedulerX-0.0.3/schedulerx/timer.py` & `SchedulerX-1.0.0/schedulerx/timer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-from .file_manager import FileManager
-from .service import ServiceManager
-from .run_command import CommandHandler
-from . import config
-
-import os
+from schedulerx import ServiceManager
+from schedulerx import CommandHandler
+from schedulerx import FileManager
 
 
 class TimerManager:
     """
 
     Args:
         service_manager (ServiceManager): service manager instance linked to
@@ -17,32 +14,26 @@
 
     def __init__(
         self,
         filename: str,
         on_calendar: str,
         service_manager: ServiceManager,
         description: str = "",
-        overwrite: bool = False,
     ) -> None:
-        self.logger = config.get_logger(__name__)
-        self.logger.info("created instance of TimerManager")
 
         self.filename = filename
         self.description = description
         self.on_calendar = on_calendar
         self.service_manager: ServiceManager = service_manager
-        self.overwrite = overwrite
 
-        self.file_manager = FileManager(filename=self.filename, overwrite=self.overwrite)
+        self.file_manager = FileManager(filename=self.filename)
         self.command_handler = CommandHandler()
 
     def create_timer(self):
-        self.logger.debug(f"create timer file {self.filename}")
         self.file_manager.create_file(self._get_timer_text())
-        self.logger.info(f"created timer file {self.filename}")
 
     def _get_timer_text(self):
         return f"""[Unit]
 Description={self.description}
 Requires={self.service_manager.filename}
 
 
@@ -52,31 +43,30 @@
 
 [Install]
 WantedBy=multi-user.target
 """
 
     def start_timer(self):
         # reload daemon process
-        self.logger.debug("reload daemon process")
-        self.command_handler.run_shell_command_as_root("systemctl daemon-reload")
+        self.command_handler.run_shell_command("systemctl daemon-reload")
         # start timer
-        self.logger.debug("start timer")
-        self.command_handler.run_shell_command_as_root(
+        self.command_handler.run_shell_command(
             f"systemctl start {self.filename}"
         )
 
-        self.logger.debug("enable timer")
-        self.command_handler.run_shell_command_as_root(
+    def enable_timer(self):
+
+        # self.logger.debug("enable timer")
+        self.command_handler.run_shell_command(
             f"systemctl enable {self.filename}"
         )
 
-        self.logger.info("timer is set successfully")
-
 
 if __name__ == "__main__":
     title = "tes"
-    sm = ServiceManager(f"{title}.service", "ls")
+    sm = ServiceManager(f"{title}.service", "siir tzft from tmer")
     sm.create_service_file()
-    tm = TimerManager(f"{title}.timer", on_calendar="12:12:12", service_manager=sm)
+    tm = TimerManager(f"{title}.timer",
+                      on_calendar="12:12:12", service_manager=sm)
     tm.create_timer()
-    os.remove(f"/etc/systemd/system/{title}.service")
-    os.remove(f"/etc/systemd/system/{title}.timer")
+    # os.remove(f"/etc/systemd/system/{title}.service")
+    # os.remove(f"/etc/systemd/system/{title}.timer")
```

### Comparing `SchedulerX-0.0.3/tests/test.py` & `SchedulerX-1.0.0/tests/test.py`

 * *Files identical despite different names*

