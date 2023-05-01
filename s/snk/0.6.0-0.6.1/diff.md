# Comparing `tmp/snk-0.6.0.tar.gz` & `tmp/snk-0.6.1.tar.gz`

## Comparing `snk-0.6.0.tar` & `snk-0.6.1.tar`

### file list

```diff
@@ -1,38 +1,42 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.0/Dockerfile
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 snk-0.6.0/mkdocs.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.0/.github/workflows/mkdocs.yml
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.0/docs/index.md
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 snk-0.6.0/docs/reference/cli.md
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.0/docs/reference/errors.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.0/docs/reference/main.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.0/docs/reference/nest.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.0/snk/__about__.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 snk-0.6.0/snk/__init__.py
--rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snk-0.6.0/snk/errors.py
--rw-r--r--   0        0        0     4595 2020-02-02 00:00:00.000000 snk-0.6.0/snk/main.py
--rw-r--r--   0        0        0     9417 2020-02-02 00:00:00.000000 snk-0.6.0/snk/nest.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/__init__.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/config.py
--rw-r--r--   0        0        0    16797 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/options.py
--rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/pipeline.py
--rw-r--r--   0        0        0     4331 2020-02-02 00:00:00.000000 snk-0.6.0/snk/cli/utils.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.0/tests/.DS_Store
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 snk-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 snk-0.6.0/tests/test_nest.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 snk-0.6.0/tests/test_pipline_cli.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 snk-0.6.0/tests/test_snk.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.0/tests/utils.py
--rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/artic_v4.1.bed
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/config.yaml
--rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/cov.fasta
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/bin/snk-basic-pipeline
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/pipeline/.snk
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/pipeline/Snakefile
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.0/tests/data/pipeline/config.yaml
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 snk-0.6.0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.0/LICENSE.txt
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.0/README.md
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 snk-0.6.1/Dockerfile
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 snk-0.6.1/mkdocs.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 snk-0.6.1/.github/workflows/mkdocs.yml
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 snk-0.6.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 snk-0.6.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 snk-0.6.1/docs/CNAME
+-rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 snk-0.6.1/docs/index.md
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 snk-0.6.1/docs/reference/cli.md
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 snk-0.6.1/docs/reference/errors.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.1/docs/reference/main.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 snk-0.6.1/docs/reference/nest.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 snk-0.6.1/snk/__about__.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 snk-0.6.1/snk/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 snk-0.6.1/snk/errors.py
+-rw-r--r--   0        0        0     5247 2020-02-02 00:00:00.000000 snk-0.6.1/snk/main.py
+-rw-r--r--   0        0        0    14897 2020-02-02 00:00:00.000000 snk-0.6.1/snk/nest.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/__init__.py
+-rw-r--r--   0        0        0    14687 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/cli.py
+-rw-r--r--   0        0        0     2734 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/options.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/pipeline.py
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 snk-0.6.1/snk/cli/utils.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 snk-0.6.1/tests/.DS_Store
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 snk-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 snk-0.6.1/tests/conftest.py
+-rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 snk-0.6.1/tests/test_nest.py
+-rw-r--r--   0        0        0     1212 2020-02-02 00:00:00.000000 snk-0.6.1/tests/test_pipline_cli.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 snk-0.6.1/tests/test_snk.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 snk-0.6.1/tests/utils.py
+-rw-r--r--   0        0        0     9605 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/artic_v4.1.bed
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/config.yaml
+-rw-r--r--   0        0        0   242003 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/cov.fasta
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/bin/snk-basic-pipeline
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/pipeline/.snk
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/pipeline/Snakefile
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/pipeline/config.yaml
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 snk-0.6.1/tests/data/pipeline/profiles/base/config.yaml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 snk-0.6.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 snk-0.6.1/LICENSE.txt
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 snk-0.6.1/README.md
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 snk-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3195 2020-02-02 00:00:00.000000 snk-0.6.1/PKG-INFO
```

### Comparing `snk-0.6.0/mkdocs.yml` & `snk-0.6.1/mkdocs.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 site_name: snk
-# repo_url: https://github.com/wytamma/write-the
+repo_url: https://github.com/Wytamma/snk
 
 theme:
   name: "material"
-  # homepage: https://write-the.wytamma.com
+  homepage: https://snk.wytamma.com
   # logo: assets/logo.png
   # favicon: images/favicon.png
   palette: 
     - scheme: default
       toggle:
         icon: material/brightness-7 
         name: Switch to dark mode
```

### Comparing `snk-0.6.0/docs/index.md` & `snk-0.6.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/snk/main.py` & `snk-0.6.1/snk/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -71,23 +71,27 @@
             None, 
             help="Specify a non-standard config location."
         ),
         resource: Optional[List[Path]] = typer.Option(
             [], 
             help="Specify a resource required to run the pipeline (copied to working dir at runtime)."
         ),
+        editable: Optional[bool] = typer.Option(False, '--editable', '-e', help="Force uninstall without asking."),
     ):
     """
     Install a pipeline.
     """
     nest = Nest(snk_home=SNK_HOME, bin_dir=SNK_BIN)
+    if not nest.bin_dir_in_path():
+        bin_dir_yellow = typer.style(nest.bin_dir, fg=typer.colors.YELLOW, bold=False)
+        typer.echo(f"Please add SNK_BIN to your $PATH: {bin_dir_yellow}")
     if not Path(pipeline).exists() and not pipeline.startswith('http'):
         pipeline = f"https://github.com/{pipeline}.git"
     try:
-        installed_pipeline = nest.install(pipeline, name=name, tag=tag, config=config, resources=resource)
+        installed_pipeline = nest.install(pipeline, editable=editable, name=name, tag=tag, config=config, resources=resource)
     except PipelineExistsError as e:
         typer.secho(e, fg='red')
         raise typer.Exit()
     except PipelineNotFoundError as e:
         typer.secho(e, fg='red')
         raise typer.Exit()
     v = installed_pipeline.version
@@ -109,48 +113,53 @@
     except PipelineNotFoundError as e:
         typer.secho(e, fg='red')
         raise typer.Exit(1)
     if uninstalled:
         typer.secho(f"Successfully uninstalled {name}!", fg='green')
         
 
-@app.command()
-def update():
-    """
-    Update a pipeline.
-    """
-    raise NotImplementedError
+# @app.command()
+# def update():
+#     """
+#     Update a pipeline.
+#     """
+#     raise NotImplementedError
 
 
 @app.command()
 def list():
     """
     List the installed pipelines.
     """
     nest = Nest()
     try:
-        pipelines = os.listdir(nest.pipelines_dir)
+        pipelines = nest.pipelines
     except FileNotFoundError:
         pipelines = []
-    pprint(pipelines)
-
-
-@app.command()
-def run(        
-        pipeline: str = typer.Argument(
-            ..., help="URL or Github name (user/repo) of the pipeline to install."
-        ),
-    ):
-    """
-    Run the pipeline in a temporary environment.
-    """
-    raise NotImplementedError
-
-@app.command()
-def annotations(config: Path):
-    """Generate annotations defaults from config file"""
-    raise NotImplementedError
-
-@app.command()
-def create(name: str):
-    """Create a default project that can be installed with snk"""
-    raise NotImplementedError
+    pipeline_dir_yellow = typer.style(nest.pipelines_dir, fg=typer.colors.YELLOW, bold=False)
+    typer.echo(f"Found {len(pipelines)} pipelines in {pipeline_dir_yellow}")
+    for pipeline in pipelines:
+        v = pipeline.version
+        v = v if v else 'latest'
+        typer.echo(f"- {pipeline.name} ({v})")
+
+
+# @app.command()
+# def run(        
+#         pipeline: str = typer.Argument(
+#             ..., help="URL or Github name (user/repo) of the pipeline to install."
+#         ),
+#     ):
+#     """
+#     Run the pipeline in a temporary environment.
+#     """
+#     raise NotImplementedError
+
+# @app.command()
+# def annotations(config: Path):
+#     """Generate annotations defaults from config file"""
+#     raise NotImplementedError
+
+# @app.command()
+# def create(name: str):
+#     """Create a default project that can be installed with snk"""
+#     raise NotImplementedError
```

### Comparing `snk-0.6.0/snk/cli/config.py` & `snk-0.6.1/snk/cli/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,34 +24,26 @@
             snk_config.resources = [snk_config_path.parent / resource for resource in snk_config.resources]
             snk_config.validate_resources(snk_config.resources)
             return snk_config
         return cls()
     
     def validate_resources(self, resources):
         """
-    Validate resources.
-    Args:
-      resources (List[Path]): List of resources to validate.
-    Raises:
-      FileNotFoundError: If a resource is not found.
-    Notes:
-      This function does not modify the resources list.
-    """
+        Validate resources.
+        Args:
+            resources (List[Path]): List of resources to validate.
+        Raises:
+            FileNotFoundError: If a resource is not found.
+        Notes:
+            This function does not modify the resources list.
+        """
         for resource in resources:
             assert resource.exists(), FileNotFoundError(f"Could not find resource: {resource}")
 
     def add_resources(self, resources: List[Path], pipeline_dir_path: Path = None):
-        """
-        Add and validate resources. 
-        It takes a list of resources, and if the resource is not absolute, it appends the
-        pipeline_dir_path to the resource
-        
-        :param resources: List[Path]
-        :param pipeline_dir_path: The path to the directory containing the pipeline
-        """
         processed = []
         for resource in resources:
             if pipeline_dir_path and not resource.is_absolute():
                 resource = pipeline_dir_path / resource
             processed.append(resource)
         self.validate_resources(processed)
         self.resources.extend(processed)
```

### Comparing `snk-0.6.0/snk/cli/main.py` & `snk-0.6.1/snk/cli/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import typer
 from pathlib import Path
 from typing import Optional, List, Callable
 from datetime import datetime
 import subprocess
 import shutil
 import os
@@ -11,132 +12,18 @@
 from rich.console import Console
 from rich.syntax import Syntax
 from art import text2art
 
 
 
 from .config import SnkConfig, get_config_from_pipeline_dir, load_pipeline_snakemake_config
-from .utils import add_dynamic_options, flatten
+from .utils import add_dynamic_options, build_dynamic_cli_options, parse_config_args
 from .pipeline import Pipeline
 
 
-def convert_key_to_samkemake_format(key, value):
-    """
-    Covert key to a format that can be passed over the cli to snakemake
-    """
-    resultDict = dict()
-    parts = key.split(":")
-    d = resultDict
-    for part in parts[:-1]:
-        if part not in d:
-            d[part] = dict()
-        d = d[part]
-    d[parts[-1]] = value
-    return resultDict
-
-def serialise(d):
-    """
-    Serialises a data structure into a string.
-    Args:
-      d (any): The data structure to serialise.
-    Returns:
-      any: The serialised data structure.
-    Examples:
-      >>> serialise({'a': 1, 'b': 2})
-      {'a': '1', 'b': '2'}
-    """
-    if isinstance(d, Path) or isinstance(d, datetime):
-        return str(d)
-
-    if isinstance(d, list):
-        return [serialise(x) for x in d]
-
-    if isinstance(d, dict):
-        for k, v in d.items():
-            d.update({k: serialise(v)})
-
-    # return anything else, like a string or number
-    return d
-
-def parse_config_args(args: List[str], options):
-    """
-    Parses a list of arguments and a list of options.
-    Args:
-      args (List[str]): A list of arguments.
-      options (List[dict]): A list of options.
-    Returns:
-      (List[str], List[dict]): A tuple of parsed arguments and config.
-    Examples:
-      >>> parse_config_args(['-name', 'John', '-age', '20'], [{'name': 'name', 'default': '', 'help': '', 'type': 'str', 'required': True}, {'name': 'age', 'default': '', 'help': '', 'type': 'int', 'required': True}])
-      (['John', '20'], [{'name': 'name', 'John'}, {'age': 20}])
-    """
-    names = [op['name'] for op in options]
-    config = []
-    parsed = []
-    flag=None
-    for arg in args:
-        if flag:
-            name = flag.lstrip('-')
-            op = next(op for op in options if op['name'] == name)
-            if op['default'] == serialise(arg):
-                # skip args that don't change
-                flag=None
-                continue
-            if ":" in op['original_key']:
-                samkemake_format_config = convert_key_to_samkemake_format(op['original_key'], arg)
-                name = list(samkemake_format_config.keys())[0]
-                arg = samkemake_format_config[name]
-            # config.append(f'{name}={serialise(arg)}')
-            config.append({name: serialise(arg)})
-            flag=None
-            continue
-        if arg.startswith('-') and arg.lstrip('-') in names:
-            flag = arg
-            continue
-        parsed.append(arg)
-    return parsed, config
-
-
-def build_dynamic_cli_options(snakemake_config, snk_config: SnkConfig):
-    """
-    Builds a list of options from a snakemake config and a snk config.
-    Args:
-      snakemake_config (dict): A snakemake config.
-      snk_config (SnkConfig): A snk config.
-    Returns:
-      List[dict]: A list of options.
-    Examples:
-      >>> build_dynamic_cli_options({'name': 'John', 'age': 20}, {'annotations': {'name:name': 'name', 'name:help': '', 'name:type': 'str', 'name:required': True, 'age:name': 'age', 'age:help': '', 'age:type': 'int', 'age:required': True}})
-      [{'name': 'name', 'original_key': 'name', 'default': 'John', 'help': '', 'type': 'str', 'required': True}, {'name': 'age', 'original_key': 'age', 'default': 20, 'help': '', 'type': 'int', 'required': True}]
-    """
-    flat_config = flatten(snakemake_config)
-    options = []
-    flat_snk_annotations = flatten(snk_config.annotations)
-    for op in flat_config:
-        name = flat_snk_annotations.get(f"{op}:name", op.replace(':', '_'))
-        help = flat_snk_annotations.get(f"{op}:help", "")
-        # TODO be smarter here 
-        # look up the List type e.g. if type == list then check the frist index type 
-        # also can probably just pass the type around instead of the string?
-        param_type = flat_snk_annotations.get(f"{op}:type", f"{type(flat_config[op]).__name__}")  # TODO refactor 
-        required = flat_snk_annotations.get(f"{op}:required", False)
-        options.append(
-            {
-                'name':name.replace('-', '_'),
-                'original_key': op,
-                'default': flat_config[op],
-                'help': help,
-                'type': param_type,
-                'required': required
-            }
-        )
-    # TODO: find annotations missing from config and add them to options
-    return options
-
-
 class CLI:
     """
     Constructor for the CLI class.
     Args:
       pipeline_dir_path (Path): Path to the pipeline directory.
     Side Effects:
       Initializes the CLI class.
@@ -173,114 +60,115 @@
         callback.__doc__ = f"{self.create_logo()}"
 
         # registration 
         self.register_callback(callback, invoke_without_command=True, context_settings={"help_option_names": ["-h", "--help"]})
         self.register_command(self.info, help="Display information about current pipeline install.")
         self.register_command(self.config, help="Access the pipeline configuration.")
         self.register_command(self.env, help="Access the pipeline conda environments.")
-        self.register_command(self.script, help="Access the pipeline scripts.")
+        self.register_command(self.profile, help="Access the pipeline profiles.")
+        # self.register_command(self.script, help="Access the pipeline scripts.")
         self.register_command(
             add_dynamic_options(self.options)(self.run), 
-            help="Run the pipeline. All unrecognized arguments are parsed onto Snakemake to be used by the pipeline.", 
+            help="Run the dynamically generated pipeline CLI.\n\nAll unrecognized arguments are passed onto Snakemake.", 
             context_settings={
                 "allow_extra_args": True, 
                 "ignore_unknown_options": True, 
                 "help_option_names": ["-h", "--help"]
             }
         )
 
     def __call__(self):
         """
-    Invoke the CLI.
-    Side Effects:
-      Invokes the CLI.
-    Examples:
-      >>> CLI(Path('/path/to/pipeline'))()
-    """
+        Invoke the CLI.
+        Side Effects:
+          Invokes the CLI.
+        Examples:
+          >>> CLI(Path('/path/to/pipeline'))()
+        """
         self.app()
 
     def register_command(self, command: Callable, **command_kwargs) -> None:
         """
-    Register a command to the CLI.
-    Args:
-      command (Callable): The command to register.
-    Side Effects:
-      Registers the command to the CLI.
-    Examples:
-      >>> CLI.register_command(my_command)
-    """
+        Register a command to the CLI.
+        Args:
+          command (Callable): The command to register.
+        Side Effects:
+          Registers the command to the CLI.
+        Examples:
+          >>> CLI.register_command(my_command)
+        """
         self.app.command(**command_kwargs)(command)
 
     def register_callback(self, command: Callable, **command_kwargs) -> None:
         """
-    Register a callback to the CLI.
-    Args:
-      command (Callable): The callback to register.
-    Side Effects:
-      Registers the callback to the CLI.
-    Examples:
-      >>> CLI.register_callback(my_callback)
-    """
+        Register a callback to the CLI.
+        Args:
+          command (Callable): The callback to register.
+        Side Effects:
+          Registers the callback to the CLI.
+        Examples:
+          >>> CLI.register_callback(my_callback)
+        """
         self.app.callback(**command_kwargs)(command)
 
     def create_logo(self, font="small"):
         """
-    Create a logo for the CLI.
-    Args:
-      font (str): The font to use for the logo.
-    Returns:
-      str: The logo.
-    Examples:
-      >>> CLI.create_logo()
-    """
+        Create a logo for the CLI.
+        Args:
+          font (str): The font to use for the logo.
+        Returns:
+          str: The logo.
+        Examples:
+          >>> CLI.create_logo()
+        """
         logo = text2art(self.name, font=font)        
         doc  = f"""\b{logo}\bA Snakemake pipeline CLI generated with snk"""
         return doc
 
     def _print_snakemake_help(value: bool):
         """
-    Print the snakemake help and exit.
-    Args:
-      value (bool): If True, print the snakemake help and exit.
-    Side Effects:
-      Prints the snakemake help and exits.
-    Examples:
-      >>> CLI._print_snakemake_help(True)
-    """
+        Print the snakemake help and exit.
+        Args:
+          value (bool): If True, print the snakemake help and exit.
+        Side Effects:
+          Prints the snakemake help and exits.
+        Examples:
+          >>> CLI._print_snakemake_help(True)
+        """
         if value:
             snakemake.main("-h")
     
     def _find_snakefile(self):
-            """
-    Search possible snakefile locations.
-    Returns:
-      Path: The path to the snakefile.
-    Examples:
-      >>> CLI._find_snakefile()
-    """
-            for path in snakemake.SNAKEFILE_CHOICES:
-                if (self.pipeline.path / path).exists():
-                    return self.pipeline.path / path 
-            raise FileNotFoundError("Snakefile not found!")
+        """
+        Search possible snakefile locations.
+        Returns:
+          Path: The path to the snakefile.
+        Examples:
+          >>> CLI._find_snakefile()
+        """
+        for path in snakemake.SNAKEFILE_CHOICES:
+            if (self.pipeline.path / path).exists():
+                return self.pipeline.path / path 
+        raise FileNotFoundError("Snakefile not found!")
     
     @contextmanager
     def copy_resources(self, resources: List[Path], cleanup: bool):
         """
-    Copy resources to the current working directory.
-    Args:
-      resources (List[Path]): A list of paths to the resources to copy.
-      cleanup (bool): If True, the resources will be removed after the function exits.
-    Side Effects:
-      Copies the resources to the current working directory.
-    Returns:
-      Generator: A generator object.
-    Examples:
-      >>> with CLI.copy_resources(resources, cleanup=True):
-      ...     # do something
-    """
+        Copy resources to the current working directory.
+        Args:
+          resources (List[Path]): A list of paths to the resources to copy.
+          cleanup (bool): If True, the resources will be removed after the function exits.
+        Side Effects:
+          Copies the resources to the current working directory.
+        Returns:
+          Generator: A generator object.
+        Examples:
+          >>> with CLI.copy_resources(resources, cleanup=True):
+          ...     # do something
+        """
         copied_resources = []
 
         def copy_resource(src, dst):
             if src.is_dir():
                 shutil.copytree(src, dst)
             else:
                 shutil.copy(src, dst)
@@ -314,39 +202,42 @@
                     remove_resource(copied_resource)
 
     def run(
             self,
             ctx: typer.Context,
             target: str = typer.Argument(None, help="File to generate. If None will run the pipeline 'all' rule."),
             configfile: Path = typer.Option(None, help="Path to snakemake config file. Overrides existing config and defaults.", exists=True, dir_okay=False),
-            resource: List[Path] = typer.Option([], help="Additional resources to copy to workdir at run time."),
-            cleanup_resources: Optional[bool] = typer.Option(True, help="Delete resources once the pipeline sucessfully completes."),
-            cleanup_snakemake: Optional[bool] = typer.Option(True, help="Delete .snakemake folder once the pipeline sucessfully completes."),
-            cores:  int = typer.Option(None, help="Set the number of cores to use. If None will use all cores."),
+            resource: List[Path] = typer.Option([], "--resource", "-r", help="Additional resources to copy to workdir at run time."),
+            profile: Optional[str] = typer.Option(None, "--profile", "-p", help=f"Name of profile to use for configuring Snakemake.",),
+            force: bool = typer.Option(False, "--force", "-f", help="Force the execution of the selected target or the first rule regardless of already created output."),
+            lock: bool = typer.Option(False, "--lock", "-l", help="Lock the working directory."),
+            keep_resources: bool = typer.Option(False, "--keep-resources", "-R", help="Keep resources after pipeline completes."),
+            keep_snakemake: bool = typer.Option(False, "--keep-snakemake", "-S", help="Keep .snakemake folder after pipeline completes."),
+            cores: int = typer.Option(None, "--cores", "-c", help="Set the number of cores to use. If None will use all cores."),
             verbose: Optional[bool] = typer.Option(False, "--verbose", "-v", help="Run pipeline in verbose mode.",),
             help_snakemake: Optional[bool] = typer.Option(
                 False, "--help-snakemake", "-hs", help="Print the snakemake help and exit.", is_eager=True, callback=_print_snakemake_help, show_default=False
             ),
         ):
         """
-    Run the pipeline.
-    Args:
-      target (str): File to generate. If None will run the pipeline 'all' rule.
-      configfile (Path): Path to snakemake config file. Overrides existing config and defaults.
-      resource (List[Path]): Additional resources to copy to workdir at run time.
-      cleanup_resources (bool): Delete resources once the pipeline sucessfully completes.
-      cleanup_snakemake (bool): Delete .snakemake folder once the pipeline sucessfully completes.
-      cores (int): Set the number of cores to use. If None will use all cores.
-      verbose (bool): Run pipeline in verbose mode.
-      help_snakemake (bool): Print the snakemake help and exit.
-    Side Effects:
-      Runs the pipeline.
-    Examples:
-      >>> CLI.run(target='my_target', configfile=Path('/path/to/config.yaml'), resource=[Path('/path/to/resource')], verbose=True)
-    """
+        Run the pipeline.
+        Args:
+          target (str): File to generate. If None will run the pipeline 'all' rule.
+          configfile (Path): Path to snakemake config file. Overrides existing config and defaults.
+          resource (List[Path]): Additional resources to copy to workdir at run time.
+          keep_resources (bool): Keep resources.
+          cleanup_snakemake (bool): Keep .snakemake folder.
+          cores (int): Set the number of cores to use. If None will use all cores.
+          verbose (bool): Run pipeline in verbose mode.
+          help_snakemake (bool): Print the snakemake help and exit.
+        Side Effects:
+          Runs the pipeline.
+        Examples:
+          >>> CLI.run(target='my_target', configfile=Path('/path/to/config.yaml'), resource=[Path('/path/to/resource')], verbose=True)
+        """
         args = []
         if not cores:
             cores = 'all'
         args.extend([
             "--use-conda",
             f"--conda-prefix={self.conda_prefix_dir}",
             f"--cores={cores}",
@@ -354,17 +245,21 @@
         if not self.snakefile.exists():
             raise ValueError('Could not find Snakefile') # this should occur at install
         else:
             args.append(f"--snakefile={self.snakefile}")
         
         if not configfile:
             configfile = get_config_from_pipeline_dir(self.pipeline.path)
-        if configfile:
-            args.append(f"--configfile={configfile}")
+        args.append(f"--configfile={configfile}")
 
+        if profile:
+          found_profile = [p for p in self.pipeline.profiles if profile==p.name]
+          if found_profile:
+              profile = found_profile[0]
+          args.append(f"--profile={profile}")
         
         # Set up conda frontend
         mamba_found = True
         try:
             subprocess.run(["mamba", "--version"], capture_output=True, check=True)
         except (subprocess.CalledProcessError, FileNotFoundError):
             typer.secho("Mamba not found! Install for speed up.", fg=typer.colors.YELLOW)
@@ -374,79 +269,110 @@
         
         typer.echo(self.create_logo())
         typer.echo()
 
         if verbose:
             args.insert(0, "--verbose")
 
+        if force:
+            args.append("--force")
+
+        if not lock:
+            args.append("--nolock")
+            
         if target:
             args.append(target)
         targets_and_or_snakemake, config_dict_list = parse_config_args(ctx.args, options=self.options)
 
         args.extend(targets_and_or_snakemake)
 
-        args.extend(["--config", *[f"{list(c.keys())[0]}={list(c.values())[0]}" for c in config_dict_list]])
+        configs = [f"{list(c.keys())[0]}={list(c.values())[0]}" for c in config_dict_list]
+        if configs:
+            args.extend(["--config", *configs])
         if verbose:
             typer.secho(f"snakemake {' '.join(args)}\n", fg=typer.colors.MAGENTA)
         
         self.snk_config.add_resources(resource, self.pipeline.path)
-        with self.copy_resources(self.snk_config.resources, cleanup=cleanup_resources):
-                snakemake.main(args)
-        if cleanup_snakemake:
+        
+        with self.copy_resources(self.snk_config.resources, cleanup=not keep_resources):
+            try:
+              status = 0
+              snakemake.main(args)
+            except SystemExit as e:
+                status = e
+        if not keep_snakemake and Path(".snakemake").exists():
+            if verbose:
+              typer.secho("Deleting .snakemake folder", fg="yellow")
             shutil.rmtree(".snakemake")
+        sys.exit(status)
 
     def info(self):
         """
-    Display information about current pipeline install.
-    Returns:
-      str: A JSON string containing information about the current pipeline install.
-    Examples:
-      >>> CLI.info()
-    """
+        Display information about current pipeline install.
+        Returns:
+          str: A JSON string containing information about the current pipeline install.
+        Examples:
+          >>> CLI.info()
+        """
         import json
         info_dict = {}
         info_dict['name'] = self.pipeline.path.name
         info_dict['version'] = self.pipeline.version
         info_dict['pipeline_dir_path'] = str(self.pipeline.path)
         typer.echo(json.dumps(info_dict, indent=2))
 
     def config(self):
         """
-    Access the pipeline configuration.
-    Side Effects:
-      Prints the pipeline configuration.
-    Examples:
-      >>> CLI.config()
-    """
+        Access the pipeline configuration.
+        Side Effects:
+          Prints the pipeline configuration.
+        Examples:
+          >>> CLI.config()
+        """
         config_path = get_config_from_pipeline_dir(self.pipeline.path)
         if not config_path:
             typer.secho("Could not find config...", fg='red')
             raise typer.Exit(1)
         with open(config_path) as f:
             code = f.read()
             syntax = Syntax(code, 'yaml')
             console = Console()
             console.print(syntax)
     
+
     def env(
-        name: Optional[str] = typer.Argument(None)
+        self,
+        name: str = typer.Argument(None, help="The name of the environment."),
     ):
         """
-    Access the pipeline conda environments.
-    Args:
-      name (str): The name of the environment.
-    Examples:
-      >>> CLI.env(name='my_env')
-    """
-        raise NotImplementedError
-
-    def script(
-        name: Optional[str] = typer.Argument(None)
+        Access the pipeline conda environments.
+        Args:
+          name (str): The name of the environment.
+        Examples:
+          >>> CLI.env(name='my_env')
+        """
+        environments_dir_yellow = typer.style(self.pipeline.path / 'envs', fg=typer.colors.YELLOW)
+        typer.echo(f"Found {len(self.pipeline.environments)} environments in {environments_dir_yellow}")
+        for env in self.pipeline.environments:
+            typer.echo(f"- {env}")
+    
+    def profile(
+        self,
+        name: str = typer.Argument(None, help="The name of the profile."),
     ):
-        """
-    Access the pipeline scripts.
-    Args:
-      name (str): The name of the script.
-    Examples:
-      >>> CLI.script(name='my_script')
-    """
-        raise NotImplementedError
+        profiles_dir_yellow = typer.style(self.pipeline.path / 'profiles', fg=typer.colors.YELLOW)
+        typer.echo(f"Found {len(self.pipeline.profiles)} profiles in {profiles_dir_yellow}")
+        for profile in self.pipeline.profiles:
+            typer.echo(f"- {profile.name}")
+
+    # def script(
+    #     self,
+    #     name: Optional[str] = typer.Argument(None)
+    # ):
+    #     """
+    #     Access the pipeline scripts.
+    #     Args:
+    #       name (str): The name of the script.
+    #     Examples:
+    #       >>> CLI.script(name='my_script')
+    #     """
+    #     raise NotImplementedError
```

### Comparing `snk-0.6.0/tests/.DS_Store` & `snk-0.6.1/tests/.DS_Store`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/tests/conftest.py` & `snk-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/tests/test_nest.py` & `snk-0.6.1/tests/test_nest.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 def test_init(bin_dir, snk_home):
     nest = Nest(snk_home, bin_dir=bin_dir)
     assert nest.pipelines_dir == Path(snk_home) / 'pipelines'
     for path in [nest.pipelines_dir, nest.bin_dir, nest.snk_home]:
         assert path.exists()
 
 def test_download(nest: Nest):
-    repo = nest.download('https://github.com/Wytamma/snk-basic-pipeline.git', 'rna-seq-star-deseq2')
+    path = nest.download('https://github.com/Wytamma/snk-basic-pipeline.git', 'rna-seq-star-deseq2')
     expected_location = nest.pipelines_dir / 'rna-seq-star-deseq2'
     assert (expected_location).exists()
-    assert Path(repo.git_dir).parent == expected_location
+    assert path == expected_location
 
 def test_create_package(nest: Nest):
     test_pipeline_path = nest.pipelines_dir / 'pipeline-name'
     test_pipeline_path.mkdir()
     path = nest.create_package(pipeline_dir=test_pipeline_path)
     assert path == test_pipeline_path / 'bin' / 'pipeline-name'
```

### Comparing `snk-0.6.0/tests/utils.py` & `snk-0.6.1/tests/utils.py`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/tests/data/artic_v4.1.bed` & `snk-0.6.1/tests/data/artic_v4.1.bed`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/tests/data/config.yaml` & `snk-0.6.1/tests/data/config.yaml`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/tests/data/cov.fasta` & `snk-0.6.1/tests/data/cov.fasta`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/LICENSE.txt` & `snk-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/README.md` & `snk-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/pyproject.toml` & `snk-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snk-0.6.0/PKG-INFO` & `snk-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snk
-Version: 0.6.0
+Version: 0.6.1
 Project-URL: Documentation, https://github.com/wytamma/snk#readme
 Project-URL: Issues, https://github.com/wytamma/snk/issues
 Project-URL: Source, https://github.com/wytamma/snk
 Author-email: Wytamma Wirth <wytamma.wirth@me.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

