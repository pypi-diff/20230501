# Comparing `tmp/stackmanager-1.4.1.tar.gz` & `tmp/stackmanager-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackmanager-1.4.1.tar", last modified: Tue Dec 13 16:24:13 2022, max compression
+gzip compressed data, was "stackmanager-1.4.2.tar", last modified: Mon May  1 15:39:43 2023, max compression
```

## Comparing `stackmanager-1.4.1.tar` & `stackmanager-1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:24:13.913720 stackmanager-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2022-12-13 16:24:06.000000 stackmanager-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19224 2022-12-13 16:24:13.913720 stackmanager-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15788 2022-12-13 16:24:06.000000 stackmanager-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-13 16:24:13.913720 stackmanager-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      912 2022-12-13 16:24:06.000000 stackmanager-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:24:13.909720 stackmanager-1.4.1/stackmanager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12981 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9388 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/packager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21376 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2022-12-13 16:24:06.000000 stackmanager-1.4.1/stackmanager/uploader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-13 16:24:13.913720 stackmanager-1.4.1/stackmanager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19224 2022-12-13 16:24:13.000000 stackmanager-1.4.1/stackmanager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2022-12-13 16:24:13.000000 stackmanager-1.4.1/stackmanager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-13 16:24:13.000000 stackmanager-1.4.1/stackmanager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2022-12-13 16:24:13.000000 stackmanager-1.4.1/stackmanager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2022-12-13 16:24:13.000000 stackmanager-1.4.1/stackmanager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-13 16:24:13.000000 stackmanager-1.4.1/stackmanager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:39:43.613295 stackmanager-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-01 15:39:32.000000 stackmanager-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-01 15:39:43.613295 stackmanager-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15788 2023-05-01 15:39:32.000000 stackmanager-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:39:43.613295 stackmanager-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-01 15:39:32.000000 stackmanager-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:39:43.613295 stackmanager-1.4.2/stackmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12981 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/packager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21376 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-01 15:39:32.000000 stackmanager-1.4.2/stackmanager/uploader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:39:43.613295 stackmanager-1.4.2/stackmanager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-01 15:39:43.000000 stackmanager-1.4.2/stackmanager.egg-info/top_level.txt
```

### Comparing `stackmanager-1.4.1/LICENSE` & `stackmanager-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.1/PKG-INFO` & `stackmanager-1.4.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,387 +1,387 @@
 Metadata-Version: 2.1
 Name: stackmanager
-Version: 1.4.1
+Version: 1.4.2
 Summary: Utility to manage CloudFormation stacks using YAML configuration file
 Home-page: https://github.com/LeadingEDJE/stackmanager
 Author: Andrew May
-License: UNKNOWN
-Description: # stackmanager
-        
-        [![PyPI version](https://badge.fury.io/py/stackmanager.svg)](https://badge.fury.io/py/stackmanager)
-        [![Coverage Status](https://coveralls.io/repos/github/LeadingEDJE/stackmanager/badge.svg?branch=master)](https://coveralls.io/github/LeadingEDJE/stackmanager?branch=master)
-        [![Docker Images](https://img.shields.io/static/v1?label=docker&message=Amazon%20ECR%20Public%20Gallery&color=blue&logo=docker&style=flat)](https://gallery.ecr.aws/leadingedje/stackmanager)
-        
-        Utility to manage CloudFormation stacks based upon a Template (either local or in S3) and a YAML configuration file.
-        
-        Uses ChangeSets to create or update CloudFormation stacks, allowing the ChangeSets to either be automatically
-        applied or applied later (e.g. during a later phase of a build pipeline after review of the ChangeSet).
-        
-        > There are also some utility methods for building a lambda file zip and uploading files to S3.
-        > These are to provide some of the AWS SAM CLI functionality while fitting into the workflow and configuration
-        > style of stackmanager.
-        
-        ## Installation
-        
-        stackmanager is available as a [Python package](https://pypi.org/project/stackmanager) or a [Docker image](https://gallery.ecr.aws/leadingedje/stackmanager) based upon Debian.
-        
-        The Docker image can be used to run container jobs in Azure DevOps pipelines and potentially other CI/CD products.
-        
-        ## Configuration
-        
-        The configuration file can either be a single YAML document containing the configuration for a stack
-        for a specific environment and region, or can contain multiple documents for different deployments
-        of that stack to different environments and regions.
-        
-        ### Single Environment
-        
-        The configuration combines together the different values that are typically passed to the CloudFormation
-        command line when creating or updating a CloudFormation stack. 
-        
-        ```yaml
-        Environment: dev
-        StackName: "{{ EnvironmentCode }}-StackManager-Integration"
-        Region: us-east-1
-        Parameters:
-          Environment: "{{ Environment }}"
-        Tags:
-          Application: StackManager
-          Environment: "{{ Environment }}"
-        Variables:
-          EnvironmentCode: d
-        Template: integration/template.yaml
-        Capabilities:
-          - CAPABILITY_NAMED_IAM
-        ```
-        
-        The configuration file makes use of [Jinja2](https://palletsprojects.com/p/jinja/) templating to perform
-        replacements into the `StackName`, `Parameters` and `Tags` values using the `Environment` and `Region` values
-        and any values from the `Variables` section.
-        
-        > It's also possible to make use of Jinja2 filters, for example to lowercase the Environment to pass into a
-        > parameter that is going to be used where it's required to be lowercase (e.g. in forming a bucket name):
-        > 
-        > ```yaml
-        > Parameters:
-        >   LowerEnvironment: "{{ Environment|lower() }}" 
-        > ```
-        
-        ### Multiple Environments
-        
-        ```yaml
-        ---
-        Environment: all
-        StackName: "{{ EnvironmentCode }}-StackManager-Integration-{{ Region }}"
-        Parameters:
-          Environment: "{{ Environment }}"
-        Tags:
-          Application: StackManager
-          Environment: "{{ Environment }}"
-        Template: integration/template.yaml
-        ---
-        Environment: dev
-        Region: us-east-1
-        Variables:
-          EnvironmentCode: d
-        ---
-        Environment: dev
-        Region: us-east-2
-        Variables:
-          EnvironmentCode: d
-        ---
-        Environment: prod
-        Region: us-east-1
-        Tags:
-          CostCenter: 200
-        Variables:
-          EnvironmentCode: p
-        ---
-        Environment: prod
-        Region: us-east-2
-        Tags:
-          CostCenter: 300
-        Variables:
-          EnvironmentCode: p
-        ```
-        
-        A multi-environment configuration can be used to combine all the configurations for different versions of a stack
-        across environments and regions, using inheritance from a specially named `all` Environment to avoid the need
-        to repeat values.
-        
-        > Because of the special handling of the `all` Environment, it's not possible to deploy an environment named `all`.
-        
-        ### Supported Configuration Values
-        
-        |Name|Required|Templated|Notes|
-        |:---|:------:|:-------:|:----|
-        |Environment|Yes|No|Name of environment to be deployed|
-        |Region|Yes|No|AWS region (e.g. us-east-1) - not required for the 'all' environment|
-        |Parameters|No|Yes|Each parameter value is templated, and parameters are inherited from 'all'|
-        |Tags|No|Yes|Each tag value is templated, and tags are inherited from 'all'|
-        |Variables|No|No|Values are inherited from all and then substituted into StackName, Parameters and Tags|
-        |Capabilities|No|No|List of capabilities (e.g. CAPABILITY_IAM)
-        |Template|No|No|Can be supplied on command line, so not required in configuration
-        |TerminationProtection|No|No|Termination Protection defaults to True|
-        
-        > In `1.2.0`, Termination Protection support was added and defaults to True, set to False in config.yml to disable.
-        > When deleting a stack using stackmanager, termination protection will be automatically disabled.
-        
-        ## Usage
-        
-        Stackmanager has the following commands:
-        
-        * [`deploy`](#deploy) - Create or update a CloudFormation stack for a specific environment/region using a ChangeSet. By default exits after creating the changeset, but can `--auto-apply`.
-        * [`apply`](#apply) - Apply a previously created ChangeSet
-        * [`reject`](#reject) - Reject a previously created ChangeSet
-        * [`delete`](#delete) - Delete an existing CloudFormation stack
-        * [`status`](#status) - Print current status of Stack
-        * [`get-output`](#get-output) - Get Stack Output value
-        * [`upload`](#upload) - Uploads a local file to S3. Utility method to prevent the need to use the AWS CLI or other tools.
-        * [`build-lambda`](#build-lambda) - Build a Lambda zip file using aws-lambda-builders.
-        
-        ```
-        Usage: stackmanager [OPTIONS] COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]...
-        
-          Utility for managing CloudFormation stacks.
-        
-        Options:
-          -p, --profile TEXT  AWS Profile, will use default or environment variables if not specified
-          -r, --region TEXT   AWS Region to deploy
-          --help              Show this message and exit.
-        
-        Commands:
-          apply         Apply a CloudFormation ChangeSet to create or update a CloudFormation stack.
-          build-lambda  Build a Lambda function zip file.
-          delete        Delete a CloudFormation stack.
-          deploy        Create or update a CloudFormation stack using ChangeSets.
-          get-output    Returns matching Output value if it exists.
-          reject        Reject a CloudFormation ChangeSet, deleting the stack if in REVIEW_IN_PROGRESS status and has no other ChangeSets.
-          status        Print current status of Stack.
-          upload        Uploads a File to S3.
-        
-        ```
-        
-        The `--profile` and `--region` options can be set either on the root `stackmanager` command, or on the nested commands.
-        
-        Multiple commands can be chained together, and the sequence of `build-lambda` -> `upload` -> `deploy` can be used to
-        deploy Lambda functions.
-        
-        > The path to the Zip file generated by `build-lambda` is passed as the `--filename` option on `upload`, and
-        > the S3 bucket and key from the `upload` command is passed as parameters to the `deploy` command.
-        
-        ### deploy
-        
-        ```
-        Usage: stackmanager deploy [OPTIONS]
-        
-          Create or update a CloudFormation stack using ChangeSets.
-        
-        Options:
-          -p, --profile TEXT              AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT          YAML Configuration file  [required]
-          -e, --environment TEXT          Environment to deploy  [required]
-          -r, --region TEXT               AWS Region to deploy  [required]
-          -t, --template TEXT             Override template
-          --parameter TEXT...             Override a parameter, can be specified multiple times
-          --parameter-use-previous TEXT   Use previous value for a parameter, can be specified multiple times
-          --change-set-name TEXT          Custom ChangeSet name
-          --existing-changes [ALLOW|FAILED_ONLY|DISALLOW]
-                                          Whether deployment is allowed when there are
-                                          existing ChangeSets
-          --auto-apply                    Automatically apply created ChangeSet
-          --help                          Show this message and exit.
-        ```
-        
-        The `--parameter` argument can be supplied multiple times and requires two values (the key and the value),
-        for example:
-        
-        ```
-        stackmanager deploy --parameter LambdaBucket mybucket --parameter LambdaKey mykey ...
-        ```
-        
-        The `--parameter-use-previous` argument can be supplied multiple times and requires one value (the name of the parameter),
-        and is typically used when a previous run has supplied a `--parameter` argument either as an override or for a value
-        not included in the configuration.
-        
-        > If `--parameter` and `--parameter-use-previous` are specified for the same parameter name, the `--parameter`
-        > value will be used. 
-        
-        Existing ChangeSets, if any, will be listed for the stack and depending upon the `--existing-changes`
-        value (which defaults to `ALLOW`) this may prevent the deployment. If set to `FAILED_ONLY` then failed ChangeSets
-        will not prevent a new change from being created, but if set to `DISALLOW` any existing ChangeSets will prevent new
-        changes.
-        
-        ### apply
-        
-        ```
-        Usage: stackmanager apply [OPTIONS]
-        
-          Apply a CloudFormation ChangeSet to create or update a CloudFormation stack. 
-          If using --change-set-name then --config --environment are --region are required. 
-          If using --change-set-id no other values are required (although --profile and --region may be needed).
-        
-        Options:
-          -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT  YAML Configuration file
-          -e, --environment TEXT  Environment to deploy
-          -r, --region TEXT       AWS Region to deploy
-          --change-set-name TEXT  Name of ChangeSet to apply
-          --change-set-id TEXT    Identifier of ChangeSet to apply
-          --help                  Show this message and exit.
-        ```
-        
-        _(since 0.7.0)_ Using `--change-set-id` allows you to apply a ChangeSet without loading the configuration.
-        This can be useful in a CI/CD pipeline as this may avoid the need to checkout the repository for applying a change.
-        
-        ### reject
-        
-        ```
-        Usage: stackmanager reject [OPTIONS]
-        
-          Reject a CloudFormation ChangeSet, deleting the stack if in REVIEW_IN_PROGRESS status and has no other ChangeSets. 
-          If using --change-set-name then --config --environment are --region are required. 
-          If using --change-set-id no other values are required (although --profile and --region may be needed).
-        
-        Options:
-          -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT  YAML Configuration file
-          -e, --environment TEXT  Environment for stack
-          -r, --region TEXT       AWS Region for stack
-          --change-set-name TEXT  Name of ChangeSet to reject
-          --change-set-id TEXT    Identifier of ChangeSet to reject
-          --help                  Show this message and exit.
-        ```
-        
-        ### delete
-        
-        ```
-        Usage: stackmanager delete [OPTIONS]
-        
-          Delete a CloudFormation stack.
-        
-        Options:
-          -p, --profile TEXT       AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT   YAML Configuration file  [required]
-          -e, --environment TEXT   Environment to deploy  [required]
-          -r, --region TEXT        AWS Region to deploy  [required]
-          --retain-resources TEXT  Logical Ids of resources to retain
-          -Y, --yes                Confirm the action without prompting.
-          --help                   Show this message and exit.
-        ```
-        
-        > Since `1.2.0` deletion requires a confirmation, either interactively or by supplying the `-Y`/`--yes` option.
-        > Deletion also now automatically removes termination protection (the logic being that you've confirmed you want to delete).
-        
-        ### get-output
-        
-        Sometimes it's necessary to get an output value from a stack to pass to something else.
-        While SSM parameter store or CloudFormation exports are a preferred way to pass values between stacks, this can be used
-        to pass a value from one stackmanager execution to another (e.g. when they are in different regions):
-        
-        ```
-        myoutput=$(stackmanger get-output -e dev -r us-east-1 -c mystack.yml -o OutputKey)
-        ```
-        
-        The output value will be the only value written to stdout.
-        
-        If the stack does not exist, or a matching output does not exist an error will be printed to stderr and the return
-        code will be -1.
-        
-        ```
-        Usage: stackmanager get-output [OPTIONS]
-        
-          Returns matching Output value if it exists.
-        
-        Options:
-          -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT  YAML Configuration file  [required]
-          -e, --environment TEXT  Environment to deploy  [required]
-          -r, --region TEXT       AWS Region to deploy
-          -o, --output-key TEXT   Output Key  [required]
-          --help                  Show this message and exit.
-        ```
-        
-        ### status
-        
-        ```
-        Usage: stackmanager status [OPTIONS]
-        
-          Print current status of Stack. Includes pending ChangeSets and recent events.
-        
-        Options:
-          -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT  YAML Configuration file  [required]
-          -e, --environment TEXT  Environment to deploy  [required]
-          -r, --region TEXT       AWS Region to deploy  [required]
-          --event-days INTEGER    Number of days of events to include in output
-          --help                  Show this message and exit.
-        ```
-        
-        ### upload
-        
-        ```
-        Usage: stackmanager upload [OPTIONS]
-        
-          Uploads a File to S3. This might be a large CloudFormation template, or a
-          Lambda zip file. Can be chained into the deploy command where it pre-populates 
-          parameters for the uploaded file.
-        
-        Options:
-          -p, --profile TEXT       AWS Profile, will use default or environment variables if not specified
-          -r, --region TEXT        AWS Region to upload to
-          -f, --filename TEXT      File to upload
-          -b, --bucket TEXT        Bucket to upload to  [required]
-          -k, --key TEXT           Key to upload to  [required]
-          --bucket-parameter TEXT  CloudFormation parameter for Bucket
-          --key-parameter TEXT     CloudFormation parameter for Key
-          --help                   Show this message and exit.
-        ```
-        
-        ### build-lambda
-        
-        ```
-        Usage: stackmanager build-lambda [OPTIONS]
-        
-          Build a Lambda function zip file. Can be chained into the upload command
-          where it pre-populates the --filename option.
-        
-        Options:
-          -s, --source-dir TEXT  Source directory  [required]
-          -o, --output-dir TEXT  Output directory  [required]
-          --runtime TEXT         Lambda Runtime  [required]
-          --archive-name TEXT    Override archive name (defaults to source directory name)
-          --help                 Show this message and exit.
-        ```
-        
-        ## CI/CD Pipeline support
-        
-        ### Azure DevOps
-        
-        Stackmanager will automatically detect when it is running in an Azure DevOps pipeline by looking for the 
-        `SYSTEM_TEAMPROJECTID` environment variable.
-        
-        It will print `##vso` strings under the following circumstances:
-        
-        * `deploy` has created a ChangeSet and it has not been auto-applied: \
-          Sets two variables for the ChangeSet name and identifier. These default to `change_set_name` and `change_set_id`
-          _(since 0.7.0)_ but the name of these variables can be changed with the `CHANGE_SET_NAME_VARIABLE` and 
-          `CHANGE_SET_ID_VARIABLE` environment variables. These values can be used with the `apply` command in a later stage.
-        * `deploy` has created a ChangeSet but it contains no changes:\
-           This logs a warning (`##vso[task.logissue]`) and sets the status to `SucceededWithIssues` (`##vso[task.complete]`)
-           allowing following steps/jobs/stages to be skipped by checking for the `SucceededStatus` in a condition.
-        * `deploy` or `apply` fails when applying a ChangeSet: \
-           This logs an error (`##vso[task.logissue]`)
-        
-        ## Additional Configuration
-        
-        > Future plans are to have a global configuration or a larger set of environment variables that can configure
-        > behavior.
-        
-        By default displayed timestamps (e.g. for CloudFormation events) will be displayed in the detected local timezone
-        including the timezone offset. If you specify a timezone using the `STACKMANAGER_TIMEZONE` environment variable
-        then this will be used instead and the timezone offset will be omitted. Olson Timezones (e.g. America/New_York)
-        are supported.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# stackmanager
+
+[![PyPI version](https://badge.fury.io/py/stackmanager.svg)](https://badge.fury.io/py/stackmanager)
+[![Coverage Status](https://coveralls.io/repos/github/LeadingEDJE/stackmanager/badge.svg?branch=master)](https://coveralls.io/github/LeadingEDJE/stackmanager?branch=master)
+[![Docker Images](https://img.shields.io/static/v1?label=docker&message=Amazon%20ECR%20Public%20Gallery&color=blue&logo=docker&style=flat)](https://gallery.ecr.aws/leadingedje/stackmanager)
+
+Utility to manage CloudFormation stacks based upon a Template (either local or in S3) and a YAML configuration file.
+
+Uses ChangeSets to create or update CloudFormation stacks, allowing the ChangeSets to either be automatically
+applied or applied later (e.g. during a later phase of a build pipeline after review of the ChangeSet).
+
+> There are also some utility methods for building a lambda file zip and uploading files to S3.
+> These are to provide some of the AWS SAM CLI functionality while fitting into the workflow and configuration
+> style of stackmanager.
+
+## Installation
+
+stackmanager is available as a [Python package](https://pypi.org/project/stackmanager) or a [Docker image](https://gallery.ecr.aws/leadingedje/stackmanager) based upon Debian.
+
+The Docker image can be used to run container jobs in Azure DevOps pipelines and potentially other CI/CD products.
+
+## Configuration
+
+The configuration file can either be a single YAML document containing the configuration for a stack
+for a specific environment and region, or can contain multiple documents for different deployments
+of that stack to different environments and regions.
+
+### Single Environment
+
+The configuration combines together the different values that are typically passed to the CloudFormation
+command line when creating or updating a CloudFormation stack. 
+
+```yaml
+Environment: dev
+StackName: "{{ EnvironmentCode }}-StackManager-Integration"
+Region: us-east-1
+Parameters:
+  Environment: "{{ Environment }}"
+Tags:
+  Application: StackManager
+  Environment: "{{ Environment }}"
+Variables:
+  EnvironmentCode: d
+Template: integration/template.yaml
+Capabilities:
+  - CAPABILITY_NAMED_IAM
+```
+
+The configuration file makes use of [Jinja2](https://palletsprojects.com/p/jinja/) templating to perform
+replacements into the `StackName`, `Parameters` and `Tags` values using the `Environment` and `Region` values
+and any values from the `Variables` section.
+
+> It's also possible to make use of Jinja2 filters, for example to lowercase the Environment to pass into a
+> parameter that is going to be used where it's required to be lowercase (e.g. in forming a bucket name):
+> 
+> ```yaml
+> Parameters:
+>   LowerEnvironment: "{{ Environment|lower() }}" 
+> ```
+
+### Multiple Environments
+
+```yaml
+---
+Environment: all
+StackName: "{{ EnvironmentCode }}-StackManager-Integration-{{ Region }}"
+Parameters:
+  Environment: "{{ Environment }}"
+Tags:
+  Application: StackManager
+  Environment: "{{ Environment }}"
+Template: integration/template.yaml
+---
+Environment: dev
+Region: us-east-1
+Variables:
+  EnvironmentCode: d
+---
+Environment: dev
+Region: us-east-2
+Variables:
+  EnvironmentCode: d
+---
+Environment: prod
+Region: us-east-1
+Tags:
+  CostCenter: 200
+Variables:
+  EnvironmentCode: p
+---
+Environment: prod
+Region: us-east-2
+Tags:
+  CostCenter: 300
+Variables:
+  EnvironmentCode: p
+```
+
+A multi-environment configuration can be used to combine all the configurations for different versions of a stack
+across environments and regions, using inheritance from a specially named `all` Environment to avoid the need
+to repeat values.
+
+> Because of the special handling of the `all` Environment, it's not possible to deploy an environment named `all`.
+
+### Supported Configuration Values
+
+|Name|Required|Templated|Notes|
+|:---|:------:|:-------:|:----|
+|Environment|Yes|No|Name of environment to be deployed|
+|Region|Yes|No|AWS region (e.g. us-east-1) - not required for the 'all' environment|
+|Parameters|No|Yes|Each parameter value is templated, and parameters are inherited from 'all'|
+|Tags|No|Yes|Each tag value is templated, and tags are inherited from 'all'|
+|Variables|No|No|Values are inherited from all and then substituted into StackName, Parameters and Tags|
+|Capabilities|No|No|List of capabilities (e.g. CAPABILITY_IAM)
+|Template|No|No|Can be supplied on command line, so not required in configuration
+|TerminationProtection|No|No|Termination Protection defaults to True|
+
+> In `1.2.0`, Termination Protection support was added and defaults to True, set to False in config.yml to disable.
+> When deleting a stack using stackmanager, termination protection will be automatically disabled.
+
+## Usage
+
+Stackmanager has the following commands:
+
+* [`deploy`](#deploy) - Create or update a CloudFormation stack for a specific environment/region using a ChangeSet. By default exits after creating the changeset, but can `--auto-apply`.
+* [`apply`](#apply) - Apply a previously created ChangeSet
+* [`reject`](#reject) - Reject a previously created ChangeSet
+* [`delete`](#delete) - Delete an existing CloudFormation stack
+* [`status`](#status) - Print current status of Stack
+* [`get-output`](#get-output) - Get Stack Output value
+* [`upload`](#upload) - Uploads a local file to S3. Utility method to prevent the need to use the AWS CLI or other tools.
+* [`build-lambda`](#build-lambda) - Build a Lambda zip file using aws-lambda-builders.
+
+```
+Usage: stackmanager [OPTIONS] COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]...
+
+  Utility for managing CloudFormation stacks.
+
+Options:
+  -p, --profile TEXT  AWS Profile, will use default or environment variables if not specified
+  -r, --region TEXT   AWS Region to deploy
+  --help              Show this message and exit.
+
+Commands:
+  apply         Apply a CloudFormation ChangeSet to create or update a CloudFormation stack.
+  build-lambda  Build a Lambda function zip file.
+  delete        Delete a CloudFormation stack.
+  deploy        Create or update a CloudFormation stack using ChangeSets.
+  get-output    Returns matching Output value if it exists.
+  reject        Reject a CloudFormation ChangeSet, deleting the stack if in REVIEW_IN_PROGRESS status and has no other ChangeSets.
+  status        Print current status of Stack.
+  upload        Uploads a File to S3.
+
+```
+
+The `--profile` and `--region` options can be set either on the root `stackmanager` command, or on the nested commands.
+
+Multiple commands can be chained together, and the sequence of `build-lambda` -> `upload` -> `deploy` can be used to
+deploy Lambda functions.
+
+> The path to the Zip file generated by `build-lambda` is passed as the `--filename` option on `upload`, and
+> the S3 bucket and key from the `upload` command is passed as parameters to the `deploy` command.
+
+### deploy
+
+```
+Usage: stackmanager deploy [OPTIONS]
+
+  Create or update a CloudFormation stack using ChangeSets.
+
+Options:
+  -p, --profile TEXT              AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT          YAML Configuration file  [required]
+  -e, --environment TEXT          Environment to deploy  [required]
+  -r, --region TEXT               AWS Region to deploy  [required]
+  -t, --template TEXT             Override template
+  --parameter TEXT...             Override a parameter, can be specified multiple times
+  --parameter-use-previous TEXT   Use previous value for a parameter, can be specified multiple times
+  --change-set-name TEXT          Custom ChangeSet name
+  --existing-changes [ALLOW|FAILED_ONLY|DISALLOW]
+                                  Whether deployment is allowed when there are
+                                  existing ChangeSets
+  --auto-apply                    Automatically apply created ChangeSet
+  --help                          Show this message and exit.
+```
+
+The `--parameter` argument can be supplied multiple times and requires two values (the key and the value),
+for example:
+
+```
+stackmanager deploy --parameter LambdaBucket mybucket --parameter LambdaKey mykey ...
+```
+
+The `--parameter-use-previous` argument can be supplied multiple times and requires one value (the name of the parameter),
+and is typically used when a previous run has supplied a `--parameter` argument either as an override or for a value
+not included in the configuration.
+
+> If `--parameter` and `--parameter-use-previous` are specified for the same parameter name, the `--parameter`
+> value will be used. 
+
+Existing ChangeSets, if any, will be listed for the stack and depending upon the `--existing-changes`
+value (which defaults to `ALLOW`) this may prevent the deployment. If set to `FAILED_ONLY` then failed ChangeSets
+will not prevent a new change from being created, but if set to `DISALLOW` any existing ChangeSets will prevent new
+changes.
+
+### apply
+
+```
+Usage: stackmanager apply [OPTIONS]
+
+  Apply a CloudFormation ChangeSet to create or update a CloudFormation stack. 
+  If using --change-set-name then --config --environment are --region are required. 
+  If using --change-set-id no other values are required (although --profile and --region may be needed).
+
+Options:
+  -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT  YAML Configuration file
+  -e, --environment TEXT  Environment to deploy
+  -r, --region TEXT       AWS Region to deploy
+  --change-set-name TEXT  Name of ChangeSet to apply
+  --change-set-id TEXT    Identifier of ChangeSet to apply
+  --help                  Show this message and exit.
+```
+
+_(since 0.7.0)_ Using `--change-set-id` allows you to apply a ChangeSet without loading the configuration.
+This can be useful in a CI/CD pipeline as this may avoid the need to checkout the repository for applying a change.
+
+### reject
+
+```
+Usage: stackmanager reject [OPTIONS]
+
+  Reject a CloudFormation ChangeSet, deleting the stack if in REVIEW_IN_PROGRESS status and has no other ChangeSets. 
+  If using --change-set-name then --config --environment are --region are required. 
+  If using --change-set-id no other values are required (although --profile and --region may be needed).
+
+Options:
+  -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT  YAML Configuration file
+  -e, --environment TEXT  Environment for stack
+  -r, --region TEXT       AWS Region for stack
+  --change-set-name TEXT  Name of ChangeSet to reject
+  --change-set-id TEXT    Identifier of ChangeSet to reject
+  --help                  Show this message and exit.
+```
+
+### delete
+
+```
+Usage: stackmanager delete [OPTIONS]
+
+  Delete a CloudFormation stack.
+
+Options:
+  -p, --profile TEXT       AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT   YAML Configuration file  [required]
+  -e, --environment TEXT   Environment to deploy  [required]
+  -r, --region TEXT        AWS Region to deploy  [required]
+  --retain-resources TEXT  Logical Ids of resources to retain
+  -Y, --yes                Confirm the action without prompting.
+  --help                   Show this message and exit.
+```
+
+> Since `1.2.0` deletion requires a confirmation, either interactively or by supplying the `-Y`/`--yes` option.
+> Deletion also now automatically removes termination protection (the logic being that you've confirmed you want to delete).
+
+### get-output
+
+Sometimes it's necessary to get an output value from a stack to pass to something else.
+While SSM parameter store or CloudFormation exports are a preferred way to pass values between stacks, this can be used
+to pass a value from one stackmanager execution to another (e.g. when they are in different regions):
+
+```
+myoutput=$(stackmanger get-output -e dev -r us-east-1 -c mystack.yml -o OutputKey)
+```
+
+The output value will be the only value written to stdout.
+
+If the stack does not exist, or a matching output does not exist an error will be printed to stderr and the return
+code will be -1.
+
+```
+Usage: stackmanager get-output [OPTIONS]
+
+  Returns matching Output value if it exists.
+
+Options:
+  -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT  YAML Configuration file  [required]
+  -e, --environment TEXT  Environment to deploy  [required]
+  -r, --region TEXT       AWS Region to deploy
+  -o, --output-key TEXT   Output Key  [required]
+  --help                  Show this message and exit.
+```
+
+### status
+
+```
+Usage: stackmanager status [OPTIONS]
+
+  Print current status of Stack. Includes pending ChangeSets and recent events.
+
+Options:
+  -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT  YAML Configuration file  [required]
+  -e, --environment TEXT  Environment to deploy  [required]
+  -r, --region TEXT       AWS Region to deploy  [required]
+  --event-days INTEGER    Number of days of events to include in output
+  --help                  Show this message and exit.
+```
+
+### upload
+
+```
+Usage: stackmanager upload [OPTIONS]
+
+  Uploads a File to S3. This might be a large CloudFormation template, or a
+  Lambda zip file. Can be chained into the deploy command where it pre-populates 
+  parameters for the uploaded file.
+
+Options:
+  -p, --profile TEXT       AWS Profile, will use default or environment variables if not specified
+  -r, --region TEXT        AWS Region to upload to
+  -f, --filename TEXT      File to upload
+  -b, --bucket TEXT        Bucket to upload to  [required]
+  -k, --key TEXT           Key to upload to  [required]
+  --bucket-parameter TEXT  CloudFormation parameter for Bucket
+  --key-parameter TEXT     CloudFormation parameter for Key
+  --help                   Show this message and exit.
+```
+
+### build-lambda
+
+```
+Usage: stackmanager build-lambda [OPTIONS]
+
+  Build a Lambda function zip file. Can be chained into the upload command
+  where it pre-populates the --filename option.
+
+Options:
+  -s, --source-dir TEXT  Source directory  [required]
+  -o, --output-dir TEXT  Output directory  [required]
+  --runtime TEXT         Lambda Runtime  [required]
+  --archive-name TEXT    Override archive name (defaults to source directory name)
+  --help                 Show this message and exit.
+```
+
+## CI/CD Pipeline support
+
+### Azure DevOps
+
+Stackmanager will automatically detect when it is running in an Azure DevOps pipeline by looking for the 
+`SYSTEM_TEAMPROJECTID` environment variable.
+
+It will print `##vso` strings under the following circumstances:
+
+* `deploy` has created a ChangeSet and it has not been auto-applied: \
+  Sets two variables for the ChangeSet name and identifier. These default to `change_set_name` and `change_set_id`
+  _(since 0.7.0)_ but the name of these variables can be changed with the `CHANGE_SET_NAME_VARIABLE` and 
+  `CHANGE_SET_ID_VARIABLE` environment variables. These values can be used with the `apply` command in a later stage.
+* `deploy` has created a ChangeSet but it contains no changes:\
+   This logs a warning (`##vso[task.logissue]`) and sets the status to `SucceededWithIssues` (`##vso[task.complete]`)
+   allowing following steps/jobs/stages to be skipped by checking for the `SucceededStatus` in a condition.
+* `deploy` or `apply` fails when applying a ChangeSet: \
+   This logs an error (`##vso[task.logissue]`)
+
+## Additional Configuration
+
+> Future plans are to have a global configuration or a larger set of environment variables that can configure
+> behavior.
+
+By default displayed timestamps (e.g. for CloudFormation events) will be displayed in the detected local timezone
+including the timezone offset. If you specify a timezone using the `STACKMANAGER_TIMEZONE` environment variable
+then this will be used instead and the timezone offset will be omitted. Olson Timezones (e.g. America/New_York)
+are supported.
```

### Comparing `stackmanager-1.4.1/README.md` & `stackmanager-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.1/setup.py` & `stackmanager-1.4.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     packages=['stackmanager'],
     install_requires=[
         'Click',
         'boto3',
         'pyyaml',
         'tabulate',
         'jinja2',
-        'aws-lambda-builders>=1.23.0',
+        'aws-lambda-builders>=1.30.0',
         'arrow'
     ],
     entry_points='''
         [console_scripts]
         stackmanager=stackmanager.cli:cli
     ''',
     classifiers=[
```

### Comparing `stackmanager-1.4.1/stackmanager/cli.py` & `stackmanager-1.4.2/stackmanager/cli.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.1/stackmanager/config.py` & `stackmanager-1.4.2/stackmanager/config.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.1/stackmanager/loader.py` & `stackmanager-1.4.2/stackmanager/loader.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.1/stackmanager/messages.py` & `stackmanager-1.4.2/stackmanager/messages.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.1/stackmanager/packager.py` & `stackmanager-1.4.2/stackmanager/packager.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,25 +20,27 @@
 GO_MOD_CONFIG = CONFIG(language='go', dependency_manager='modules', manifest_name='go.mod')
 
 RUNTIMES = {
     'python3.6': PYTHON_PIP_CONFIG,
     'python3.7': PYTHON_PIP_CONFIG,
     'python3.8': PYTHON_PIP_CONFIG,
     'python3.9': PYTHON_PIP_CONFIG,
+    'python3.10': PYTHON_PIP_CONFIG,
     'dotnetcore3.1': DOTNET_CLIPACKAGE_CONFIG,
     'dotnet6': DOTNET_CLIPACKAGE_CONFIG,
     'nodejs12.x': NODEJS_NPM_CONFIG,
     'nodejs14.x': NODEJS_NPM_CONFIG,
     'nodejs16.x': NODEJS_NPM_CONFIG,
     'nodejs18.x': NODEJS_NPM_CONFIG,
     'ruby2.7': RUBY_BUNDLER_CONFIG,
     'go1.x': GO_MOD_CONFIG,
     'java8': [JAVA_MAVEN_CONFIG, JAVA_GRADLE_CONFIG, JAVA_KOTLIN_GRADLE_CONFIG],
     'java8.al2': [JAVA_MAVEN_CONFIG, JAVA_GRADLE_CONFIG, JAVA_KOTLIN_GRADLE_CONFIG],
-    'java11': [JAVA_MAVEN_CONFIG, JAVA_GRADLE_CONFIG, JAVA_KOTLIN_GRADLE_CONFIG]
+    'java11': [JAVA_MAVEN_CONFIG, JAVA_GRADLE_CONFIG, JAVA_KOTLIN_GRADLE_CONFIG],
+    'java17': [JAVA_MAVEN_CONFIG, JAVA_GRADLE_CONFIG, JAVA_KOTLIN_GRADLE_CONFIG]
 }
 
 # Configure logging for aws_lambda_builders
 log_stream_handler = logging.StreamHandler()
 log_stream_handler.setLevel(logging.DEBUG)
 log_stream_handler.setFormatter(logging.Formatter("%(message)s"))
```

### Comparing `stackmanager-1.4.1/stackmanager/runner.py` & `stackmanager-1.4.2/stackmanager/runner.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.1/stackmanager/status.py` & `stackmanager-1.4.2/stackmanager/status.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.1/stackmanager/uploader.py` & `stackmanager-1.4.2/stackmanager/uploader.py`

 * *Files identical despite different names*

### Comparing `stackmanager-1.4.1/stackmanager.egg-info/PKG-INFO` & `stackmanager-1.4.2/stackmanager.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,387 +1,387 @@
 Metadata-Version: 2.1
 Name: stackmanager
-Version: 1.4.1
+Version: 1.4.2
 Summary: Utility to manage CloudFormation stacks using YAML configuration file
 Home-page: https://github.com/LeadingEDJE/stackmanager
 Author: Andrew May
-License: UNKNOWN
-Description: # stackmanager
-        
-        [![PyPI version](https://badge.fury.io/py/stackmanager.svg)](https://badge.fury.io/py/stackmanager)
-        [![Coverage Status](https://coveralls.io/repos/github/LeadingEDJE/stackmanager/badge.svg?branch=master)](https://coveralls.io/github/LeadingEDJE/stackmanager?branch=master)
-        [![Docker Images](https://img.shields.io/static/v1?label=docker&message=Amazon%20ECR%20Public%20Gallery&color=blue&logo=docker&style=flat)](https://gallery.ecr.aws/leadingedje/stackmanager)
-        
-        Utility to manage CloudFormation stacks based upon a Template (either local or in S3) and a YAML configuration file.
-        
-        Uses ChangeSets to create or update CloudFormation stacks, allowing the ChangeSets to either be automatically
-        applied or applied later (e.g. during a later phase of a build pipeline after review of the ChangeSet).
-        
-        > There are also some utility methods for building a lambda file zip and uploading files to S3.
-        > These are to provide some of the AWS SAM CLI functionality while fitting into the workflow and configuration
-        > style of stackmanager.
-        
-        ## Installation
-        
-        stackmanager is available as a [Python package](https://pypi.org/project/stackmanager) or a [Docker image](https://gallery.ecr.aws/leadingedje/stackmanager) based upon Debian.
-        
-        The Docker image can be used to run container jobs in Azure DevOps pipelines and potentially other CI/CD products.
-        
-        ## Configuration
-        
-        The configuration file can either be a single YAML document containing the configuration for a stack
-        for a specific environment and region, or can contain multiple documents for different deployments
-        of that stack to different environments and regions.
-        
-        ### Single Environment
-        
-        The configuration combines together the different values that are typically passed to the CloudFormation
-        command line when creating or updating a CloudFormation stack. 
-        
-        ```yaml
-        Environment: dev
-        StackName: "{{ EnvironmentCode }}-StackManager-Integration"
-        Region: us-east-1
-        Parameters:
-          Environment: "{{ Environment }}"
-        Tags:
-          Application: StackManager
-          Environment: "{{ Environment }}"
-        Variables:
-          EnvironmentCode: d
-        Template: integration/template.yaml
-        Capabilities:
-          - CAPABILITY_NAMED_IAM
-        ```
-        
-        The configuration file makes use of [Jinja2](https://palletsprojects.com/p/jinja/) templating to perform
-        replacements into the `StackName`, `Parameters` and `Tags` values using the `Environment` and `Region` values
-        and any values from the `Variables` section.
-        
-        > It's also possible to make use of Jinja2 filters, for example to lowercase the Environment to pass into a
-        > parameter that is going to be used where it's required to be lowercase (e.g. in forming a bucket name):
-        > 
-        > ```yaml
-        > Parameters:
-        >   LowerEnvironment: "{{ Environment|lower() }}" 
-        > ```
-        
-        ### Multiple Environments
-        
-        ```yaml
-        ---
-        Environment: all
-        StackName: "{{ EnvironmentCode }}-StackManager-Integration-{{ Region }}"
-        Parameters:
-          Environment: "{{ Environment }}"
-        Tags:
-          Application: StackManager
-          Environment: "{{ Environment }}"
-        Template: integration/template.yaml
-        ---
-        Environment: dev
-        Region: us-east-1
-        Variables:
-          EnvironmentCode: d
-        ---
-        Environment: dev
-        Region: us-east-2
-        Variables:
-          EnvironmentCode: d
-        ---
-        Environment: prod
-        Region: us-east-1
-        Tags:
-          CostCenter: 200
-        Variables:
-          EnvironmentCode: p
-        ---
-        Environment: prod
-        Region: us-east-2
-        Tags:
-          CostCenter: 300
-        Variables:
-          EnvironmentCode: p
-        ```
-        
-        A multi-environment configuration can be used to combine all the configurations for different versions of a stack
-        across environments and regions, using inheritance from a specially named `all` Environment to avoid the need
-        to repeat values.
-        
-        > Because of the special handling of the `all` Environment, it's not possible to deploy an environment named `all`.
-        
-        ### Supported Configuration Values
-        
-        |Name|Required|Templated|Notes|
-        |:---|:------:|:-------:|:----|
-        |Environment|Yes|No|Name of environment to be deployed|
-        |Region|Yes|No|AWS region (e.g. us-east-1) - not required for the 'all' environment|
-        |Parameters|No|Yes|Each parameter value is templated, and parameters are inherited from 'all'|
-        |Tags|No|Yes|Each tag value is templated, and tags are inherited from 'all'|
-        |Variables|No|No|Values are inherited from all and then substituted into StackName, Parameters and Tags|
-        |Capabilities|No|No|List of capabilities (e.g. CAPABILITY_IAM)
-        |Template|No|No|Can be supplied on command line, so not required in configuration
-        |TerminationProtection|No|No|Termination Protection defaults to True|
-        
-        > In `1.2.0`, Termination Protection support was added and defaults to True, set to False in config.yml to disable.
-        > When deleting a stack using stackmanager, termination protection will be automatically disabled.
-        
-        ## Usage
-        
-        Stackmanager has the following commands:
-        
-        * [`deploy`](#deploy) - Create or update a CloudFormation stack for a specific environment/region using a ChangeSet. By default exits after creating the changeset, but can `--auto-apply`.
-        * [`apply`](#apply) - Apply a previously created ChangeSet
-        * [`reject`](#reject) - Reject a previously created ChangeSet
-        * [`delete`](#delete) - Delete an existing CloudFormation stack
-        * [`status`](#status) - Print current status of Stack
-        * [`get-output`](#get-output) - Get Stack Output value
-        * [`upload`](#upload) - Uploads a local file to S3. Utility method to prevent the need to use the AWS CLI or other tools.
-        * [`build-lambda`](#build-lambda) - Build a Lambda zip file using aws-lambda-builders.
-        
-        ```
-        Usage: stackmanager [OPTIONS] COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]...
-        
-          Utility for managing CloudFormation stacks.
-        
-        Options:
-          -p, --profile TEXT  AWS Profile, will use default or environment variables if not specified
-          -r, --region TEXT   AWS Region to deploy
-          --help              Show this message and exit.
-        
-        Commands:
-          apply         Apply a CloudFormation ChangeSet to create or update a CloudFormation stack.
-          build-lambda  Build a Lambda function zip file.
-          delete        Delete a CloudFormation stack.
-          deploy        Create or update a CloudFormation stack using ChangeSets.
-          get-output    Returns matching Output value if it exists.
-          reject        Reject a CloudFormation ChangeSet, deleting the stack if in REVIEW_IN_PROGRESS status and has no other ChangeSets.
-          status        Print current status of Stack.
-          upload        Uploads a File to S3.
-        
-        ```
-        
-        The `--profile` and `--region` options can be set either on the root `stackmanager` command, or on the nested commands.
-        
-        Multiple commands can be chained together, and the sequence of `build-lambda` -> `upload` -> `deploy` can be used to
-        deploy Lambda functions.
-        
-        > The path to the Zip file generated by `build-lambda` is passed as the `--filename` option on `upload`, and
-        > the S3 bucket and key from the `upload` command is passed as parameters to the `deploy` command.
-        
-        ### deploy
-        
-        ```
-        Usage: stackmanager deploy [OPTIONS]
-        
-          Create or update a CloudFormation stack using ChangeSets.
-        
-        Options:
-          -p, --profile TEXT              AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT          YAML Configuration file  [required]
-          -e, --environment TEXT          Environment to deploy  [required]
-          -r, --region TEXT               AWS Region to deploy  [required]
-          -t, --template TEXT             Override template
-          --parameter TEXT...             Override a parameter, can be specified multiple times
-          --parameter-use-previous TEXT   Use previous value for a parameter, can be specified multiple times
-          --change-set-name TEXT          Custom ChangeSet name
-          --existing-changes [ALLOW|FAILED_ONLY|DISALLOW]
-                                          Whether deployment is allowed when there are
-                                          existing ChangeSets
-          --auto-apply                    Automatically apply created ChangeSet
-          --help                          Show this message and exit.
-        ```
-        
-        The `--parameter` argument can be supplied multiple times and requires two values (the key and the value),
-        for example:
-        
-        ```
-        stackmanager deploy --parameter LambdaBucket mybucket --parameter LambdaKey mykey ...
-        ```
-        
-        The `--parameter-use-previous` argument can be supplied multiple times and requires one value (the name of the parameter),
-        and is typically used when a previous run has supplied a `--parameter` argument either as an override or for a value
-        not included in the configuration.
-        
-        > If `--parameter` and `--parameter-use-previous` are specified for the same parameter name, the `--parameter`
-        > value will be used. 
-        
-        Existing ChangeSets, if any, will be listed for the stack and depending upon the `--existing-changes`
-        value (which defaults to `ALLOW`) this may prevent the deployment. If set to `FAILED_ONLY` then failed ChangeSets
-        will not prevent a new change from being created, but if set to `DISALLOW` any existing ChangeSets will prevent new
-        changes.
-        
-        ### apply
-        
-        ```
-        Usage: stackmanager apply [OPTIONS]
-        
-          Apply a CloudFormation ChangeSet to create or update a CloudFormation stack. 
-          If using --change-set-name then --config --environment are --region are required. 
-          If using --change-set-id no other values are required (although --profile and --region may be needed).
-        
-        Options:
-          -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT  YAML Configuration file
-          -e, --environment TEXT  Environment to deploy
-          -r, --region TEXT       AWS Region to deploy
-          --change-set-name TEXT  Name of ChangeSet to apply
-          --change-set-id TEXT    Identifier of ChangeSet to apply
-          --help                  Show this message and exit.
-        ```
-        
-        _(since 0.7.0)_ Using `--change-set-id` allows you to apply a ChangeSet without loading the configuration.
-        This can be useful in a CI/CD pipeline as this may avoid the need to checkout the repository for applying a change.
-        
-        ### reject
-        
-        ```
-        Usage: stackmanager reject [OPTIONS]
-        
-          Reject a CloudFormation ChangeSet, deleting the stack if in REVIEW_IN_PROGRESS status and has no other ChangeSets. 
-          If using --change-set-name then --config --environment are --region are required. 
-          If using --change-set-id no other values are required (although --profile and --region may be needed).
-        
-        Options:
-          -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT  YAML Configuration file
-          -e, --environment TEXT  Environment for stack
-          -r, --region TEXT       AWS Region for stack
-          --change-set-name TEXT  Name of ChangeSet to reject
-          --change-set-id TEXT    Identifier of ChangeSet to reject
-          --help                  Show this message and exit.
-        ```
-        
-        ### delete
-        
-        ```
-        Usage: stackmanager delete [OPTIONS]
-        
-          Delete a CloudFormation stack.
-        
-        Options:
-          -p, --profile TEXT       AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT   YAML Configuration file  [required]
-          -e, --environment TEXT   Environment to deploy  [required]
-          -r, --region TEXT        AWS Region to deploy  [required]
-          --retain-resources TEXT  Logical Ids of resources to retain
-          -Y, --yes                Confirm the action without prompting.
-          --help                   Show this message and exit.
-        ```
-        
-        > Since `1.2.0` deletion requires a confirmation, either interactively or by supplying the `-Y`/`--yes` option.
-        > Deletion also now automatically removes termination protection (the logic being that you've confirmed you want to delete).
-        
-        ### get-output
-        
-        Sometimes it's necessary to get an output value from a stack to pass to something else.
-        While SSM parameter store or CloudFormation exports are a preferred way to pass values between stacks, this can be used
-        to pass a value from one stackmanager execution to another (e.g. when they are in different regions):
-        
-        ```
-        myoutput=$(stackmanger get-output -e dev -r us-east-1 -c mystack.yml -o OutputKey)
-        ```
-        
-        The output value will be the only value written to stdout.
-        
-        If the stack does not exist, or a matching output does not exist an error will be printed to stderr and the return
-        code will be -1.
-        
-        ```
-        Usage: stackmanager get-output [OPTIONS]
-        
-          Returns matching Output value if it exists.
-        
-        Options:
-          -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT  YAML Configuration file  [required]
-          -e, --environment TEXT  Environment to deploy  [required]
-          -r, --region TEXT       AWS Region to deploy
-          -o, --output-key TEXT   Output Key  [required]
-          --help                  Show this message and exit.
-        ```
-        
-        ### status
-        
-        ```
-        Usage: stackmanager status [OPTIONS]
-        
-          Print current status of Stack. Includes pending ChangeSets and recent events.
-        
-        Options:
-          -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
-          -c, --config-file TEXT  YAML Configuration file  [required]
-          -e, --environment TEXT  Environment to deploy  [required]
-          -r, --region TEXT       AWS Region to deploy  [required]
-          --event-days INTEGER    Number of days of events to include in output
-          --help                  Show this message and exit.
-        ```
-        
-        ### upload
-        
-        ```
-        Usage: stackmanager upload [OPTIONS]
-        
-          Uploads a File to S3. This might be a large CloudFormation template, or a
-          Lambda zip file. Can be chained into the deploy command where it pre-populates 
-          parameters for the uploaded file.
-        
-        Options:
-          -p, --profile TEXT       AWS Profile, will use default or environment variables if not specified
-          -r, --region TEXT        AWS Region to upload to
-          -f, --filename TEXT      File to upload
-          -b, --bucket TEXT        Bucket to upload to  [required]
-          -k, --key TEXT           Key to upload to  [required]
-          --bucket-parameter TEXT  CloudFormation parameter for Bucket
-          --key-parameter TEXT     CloudFormation parameter for Key
-          --help                   Show this message and exit.
-        ```
-        
-        ### build-lambda
-        
-        ```
-        Usage: stackmanager build-lambda [OPTIONS]
-        
-          Build a Lambda function zip file. Can be chained into the upload command
-          where it pre-populates the --filename option.
-        
-        Options:
-          -s, --source-dir TEXT  Source directory  [required]
-          -o, --output-dir TEXT  Output directory  [required]
-          --runtime TEXT         Lambda Runtime  [required]
-          --archive-name TEXT    Override archive name (defaults to source directory name)
-          --help                 Show this message and exit.
-        ```
-        
-        ## CI/CD Pipeline support
-        
-        ### Azure DevOps
-        
-        Stackmanager will automatically detect when it is running in an Azure DevOps pipeline by looking for the 
-        `SYSTEM_TEAMPROJECTID` environment variable.
-        
-        It will print `##vso` strings under the following circumstances:
-        
-        * `deploy` has created a ChangeSet and it has not been auto-applied: \
-          Sets two variables for the ChangeSet name and identifier. These default to `change_set_name` and `change_set_id`
-          _(since 0.7.0)_ but the name of these variables can be changed with the `CHANGE_SET_NAME_VARIABLE` and 
-          `CHANGE_SET_ID_VARIABLE` environment variables. These values can be used with the `apply` command in a later stage.
-        * `deploy` has created a ChangeSet but it contains no changes:\
-           This logs a warning (`##vso[task.logissue]`) and sets the status to `SucceededWithIssues` (`##vso[task.complete]`)
-           allowing following steps/jobs/stages to be skipped by checking for the `SucceededStatus` in a condition.
-        * `deploy` or `apply` fails when applying a ChangeSet: \
-           This logs an error (`##vso[task.logissue]`)
-        
-        ## Additional Configuration
-        
-        > Future plans are to have a global configuration or a larger set of environment variables that can configure
-        > behavior.
-        
-        By default displayed timestamps (e.g. for CloudFormation events) will be displayed in the detected local timezone
-        including the timezone offset. If you specify a timezone using the `STACKMANAGER_TIMEZONE` environment variable
-        then this will be used instead and the timezone offset will be omitted. Olson Timezones (e.g. America/New_York)
-        are supported.
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# stackmanager
+
+[![PyPI version](https://badge.fury.io/py/stackmanager.svg)](https://badge.fury.io/py/stackmanager)
+[![Coverage Status](https://coveralls.io/repos/github/LeadingEDJE/stackmanager/badge.svg?branch=master)](https://coveralls.io/github/LeadingEDJE/stackmanager?branch=master)
+[![Docker Images](https://img.shields.io/static/v1?label=docker&message=Amazon%20ECR%20Public%20Gallery&color=blue&logo=docker&style=flat)](https://gallery.ecr.aws/leadingedje/stackmanager)
+
+Utility to manage CloudFormation stacks based upon a Template (either local or in S3) and a YAML configuration file.
+
+Uses ChangeSets to create or update CloudFormation stacks, allowing the ChangeSets to either be automatically
+applied or applied later (e.g. during a later phase of a build pipeline after review of the ChangeSet).
+
+> There are also some utility methods for building a lambda file zip and uploading files to S3.
+> These are to provide some of the AWS SAM CLI functionality while fitting into the workflow and configuration
+> style of stackmanager.
+
+## Installation
+
+stackmanager is available as a [Python package](https://pypi.org/project/stackmanager) or a [Docker image](https://gallery.ecr.aws/leadingedje/stackmanager) based upon Debian.
+
+The Docker image can be used to run container jobs in Azure DevOps pipelines and potentially other CI/CD products.
+
+## Configuration
+
+The configuration file can either be a single YAML document containing the configuration for a stack
+for a specific environment and region, or can contain multiple documents for different deployments
+of that stack to different environments and regions.
+
+### Single Environment
+
+The configuration combines together the different values that are typically passed to the CloudFormation
+command line when creating or updating a CloudFormation stack. 
+
+```yaml
+Environment: dev
+StackName: "{{ EnvironmentCode }}-StackManager-Integration"
+Region: us-east-1
+Parameters:
+  Environment: "{{ Environment }}"
+Tags:
+  Application: StackManager
+  Environment: "{{ Environment }}"
+Variables:
+  EnvironmentCode: d
+Template: integration/template.yaml
+Capabilities:
+  - CAPABILITY_NAMED_IAM
+```
+
+The configuration file makes use of [Jinja2](https://palletsprojects.com/p/jinja/) templating to perform
+replacements into the `StackName`, `Parameters` and `Tags` values using the `Environment` and `Region` values
+and any values from the `Variables` section.
+
+> It's also possible to make use of Jinja2 filters, for example to lowercase the Environment to pass into a
+> parameter that is going to be used where it's required to be lowercase (e.g. in forming a bucket name):
+> 
+> ```yaml
+> Parameters:
+>   LowerEnvironment: "{{ Environment|lower() }}" 
+> ```
+
+### Multiple Environments
+
+```yaml
+---
+Environment: all
+StackName: "{{ EnvironmentCode }}-StackManager-Integration-{{ Region }}"
+Parameters:
+  Environment: "{{ Environment }}"
+Tags:
+  Application: StackManager
+  Environment: "{{ Environment }}"
+Template: integration/template.yaml
+---
+Environment: dev
+Region: us-east-1
+Variables:
+  EnvironmentCode: d
+---
+Environment: dev
+Region: us-east-2
+Variables:
+  EnvironmentCode: d
+---
+Environment: prod
+Region: us-east-1
+Tags:
+  CostCenter: 200
+Variables:
+  EnvironmentCode: p
+---
+Environment: prod
+Region: us-east-2
+Tags:
+  CostCenter: 300
+Variables:
+  EnvironmentCode: p
+```
+
+A multi-environment configuration can be used to combine all the configurations for different versions of a stack
+across environments and regions, using inheritance from a specially named `all` Environment to avoid the need
+to repeat values.
+
+> Because of the special handling of the `all` Environment, it's not possible to deploy an environment named `all`.
+
+### Supported Configuration Values
+
+|Name|Required|Templated|Notes|
+|:---|:------:|:-------:|:----|
+|Environment|Yes|No|Name of environment to be deployed|
+|Region|Yes|No|AWS region (e.g. us-east-1) - not required for the 'all' environment|
+|Parameters|No|Yes|Each parameter value is templated, and parameters are inherited from 'all'|
+|Tags|No|Yes|Each tag value is templated, and tags are inherited from 'all'|
+|Variables|No|No|Values are inherited from all and then substituted into StackName, Parameters and Tags|
+|Capabilities|No|No|List of capabilities (e.g. CAPABILITY_IAM)
+|Template|No|No|Can be supplied on command line, so not required in configuration
+|TerminationProtection|No|No|Termination Protection defaults to True|
+
+> In `1.2.0`, Termination Protection support was added and defaults to True, set to False in config.yml to disable.
+> When deleting a stack using stackmanager, termination protection will be automatically disabled.
+
+## Usage
+
+Stackmanager has the following commands:
+
+* [`deploy`](#deploy) - Create or update a CloudFormation stack for a specific environment/region using a ChangeSet. By default exits after creating the changeset, but can `--auto-apply`.
+* [`apply`](#apply) - Apply a previously created ChangeSet
+* [`reject`](#reject) - Reject a previously created ChangeSet
+* [`delete`](#delete) - Delete an existing CloudFormation stack
+* [`status`](#status) - Print current status of Stack
+* [`get-output`](#get-output) - Get Stack Output value
+* [`upload`](#upload) - Uploads a local file to S3. Utility method to prevent the need to use the AWS CLI or other tools.
+* [`build-lambda`](#build-lambda) - Build a Lambda zip file using aws-lambda-builders.
+
+```
+Usage: stackmanager [OPTIONS] COMMAND1 [ARGS]... [COMMAND2 [ARGS]...]...
+
+  Utility for managing CloudFormation stacks.
+
+Options:
+  -p, --profile TEXT  AWS Profile, will use default or environment variables if not specified
+  -r, --region TEXT   AWS Region to deploy
+  --help              Show this message and exit.
+
+Commands:
+  apply         Apply a CloudFormation ChangeSet to create or update a CloudFormation stack.
+  build-lambda  Build a Lambda function zip file.
+  delete        Delete a CloudFormation stack.
+  deploy        Create or update a CloudFormation stack using ChangeSets.
+  get-output    Returns matching Output value if it exists.
+  reject        Reject a CloudFormation ChangeSet, deleting the stack if in REVIEW_IN_PROGRESS status and has no other ChangeSets.
+  status        Print current status of Stack.
+  upload        Uploads a File to S3.
+
+```
+
+The `--profile` and `--region` options can be set either on the root `stackmanager` command, or on the nested commands.
+
+Multiple commands can be chained together, and the sequence of `build-lambda` -> `upload` -> `deploy` can be used to
+deploy Lambda functions.
+
+> The path to the Zip file generated by `build-lambda` is passed as the `--filename` option on `upload`, and
+> the S3 bucket and key from the `upload` command is passed as parameters to the `deploy` command.
+
+### deploy
+
+```
+Usage: stackmanager deploy [OPTIONS]
+
+  Create or update a CloudFormation stack using ChangeSets.
+
+Options:
+  -p, --profile TEXT              AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT          YAML Configuration file  [required]
+  -e, --environment TEXT          Environment to deploy  [required]
+  -r, --region TEXT               AWS Region to deploy  [required]
+  -t, --template TEXT             Override template
+  --parameter TEXT...             Override a parameter, can be specified multiple times
+  --parameter-use-previous TEXT   Use previous value for a parameter, can be specified multiple times
+  --change-set-name TEXT          Custom ChangeSet name
+  --existing-changes [ALLOW|FAILED_ONLY|DISALLOW]
+                                  Whether deployment is allowed when there are
+                                  existing ChangeSets
+  --auto-apply                    Automatically apply created ChangeSet
+  --help                          Show this message and exit.
+```
+
+The `--parameter` argument can be supplied multiple times and requires two values (the key and the value),
+for example:
+
+```
+stackmanager deploy --parameter LambdaBucket mybucket --parameter LambdaKey mykey ...
+```
+
+The `--parameter-use-previous` argument can be supplied multiple times and requires one value (the name of the parameter),
+and is typically used when a previous run has supplied a `--parameter` argument either as an override or for a value
+not included in the configuration.
+
+> If `--parameter` and `--parameter-use-previous` are specified for the same parameter name, the `--parameter`
+> value will be used. 
+
+Existing ChangeSets, if any, will be listed for the stack and depending upon the `--existing-changes`
+value (which defaults to `ALLOW`) this may prevent the deployment. If set to `FAILED_ONLY` then failed ChangeSets
+will not prevent a new change from being created, but if set to `DISALLOW` any existing ChangeSets will prevent new
+changes.
+
+### apply
+
+```
+Usage: stackmanager apply [OPTIONS]
+
+  Apply a CloudFormation ChangeSet to create or update a CloudFormation stack. 
+  If using --change-set-name then --config --environment are --region are required. 
+  If using --change-set-id no other values are required (although --profile and --region may be needed).
+
+Options:
+  -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT  YAML Configuration file
+  -e, --environment TEXT  Environment to deploy
+  -r, --region TEXT       AWS Region to deploy
+  --change-set-name TEXT  Name of ChangeSet to apply
+  --change-set-id TEXT    Identifier of ChangeSet to apply
+  --help                  Show this message and exit.
+```
+
+_(since 0.7.0)_ Using `--change-set-id` allows you to apply a ChangeSet without loading the configuration.
+This can be useful in a CI/CD pipeline as this may avoid the need to checkout the repository for applying a change.
+
+### reject
+
+```
+Usage: stackmanager reject [OPTIONS]
+
+  Reject a CloudFormation ChangeSet, deleting the stack if in REVIEW_IN_PROGRESS status and has no other ChangeSets. 
+  If using --change-set-name then --config --environment are --region are required. 
+  If using --change-set-id no other values are required (although --profile and --region may be needed).
+
+Options:
+  -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT  YAML Configuration file
+  -e, --environment TEXT  Environment for stack
+  -r, --region TEXT       AWS Region for stack
+  --change-set-name TEXT  Name of ChangeSet to reject
+  --change-set-id TEXT    Identifier of ChangeSet to reject
+  --help                  Show this message and exit.
+```
+
+### delete
+
+```
+Usage: stackmanager delete [OPTIONS]
+
+  Delete a CloudFormation stack.
+
+Options:
+  -p, --profile TEXT       AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT   YAML Configuration file  [required]
+  -e, --environment TEXT   Environment to deploy  [required]
+  -r, --region TEXT        AWS Region to deploy  [required]
+  --retain-resources TEXT  Logical Ids of resources to retain
+  -Y, --yes                Confirm the action without prompting.
+  --help                   Show this message and exit.
+```
+
+> Since `1.2.0` deletion requires a confirmation, either interactively or by supplying the `-Y`/`--yes` option.
+> Deletion also now automatically removes termination protection (the logic being that you've confirmed you want to delete).
+
+### get-output
+
+Sometimes it's necessary to get an output value from a stack to pass to something else.
+While SSM parameter store or CloudFormation exports are a preferred way to pass values between stacks, this can be used
+to pass a value from one stackmanager execution to another (e.g. when they are in different regions):
+
+```
+myoutput=$(stackmanger get-output -e dev -r us-east-1 -c mystack.yml -o OutputKey)
+```
+
+The output value will be the only value written to stdout.
+
+If the stack does not exist, or a matching output does not exist an error will be printed to stderr and the return
+code will be -1.
+
+```
+Usage: stackmanager get-output [OPTIONS]
+
+  Returns matching Output value if it exists.
+
+Options:
+  -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT  YAML Configuration file  [required]
+  -e, --environment TEXT  Environment to deploy  [required]
+  -r, --region TEXT       AWS Region to deploy
+  -o, --output-key TEXT   Output Key  [required]
+  --help                  Show this message and exit.
+```
+
+### status
+
+```
+Usage: stackmanager status [OPTIONS]
+
+  Print current status of Stack. Includes pending ChangeSets and recent events.
+
+Options:
+  -p, --profile TEXT      AWS Profile, will use default or environment variables if not specified
+  -c, --config-file TEXT  YAML Configuration file  [required]
+  -e, --environment TEXT  Environment to deploy  [required]
+  -r, --region TEXT       AWS Region to deploy  [required]
+  --event-days INTEGER    Number of days of events to include in output
+  --help                  Show this message and exit.
+```
+
+### upload
+
+```
+Usage: stackmanager upload [OPTIONS]
+
+  Uploads a File to S3. This might be a large CloudFormation template, or a
+  Lambda zip file. Can be chained into the deploy command where it pre-populates 
+  parameters for the uploaded file.
+
+Options:
+  -p, --profile TEXT       AWS Profile, will use default or environment variables if not specified
+  -r, --region TEXT        AWS Region to upload to
+  -f, --filename TEXT      File to upload
+  -b, --bucket TEXT        Bucket to upload to  [required]
+  -k, --key TEXT           Key to upload to  [required]
+  --bucket-parameter TEXT  CloudFormation parameter for Bucket
+  --key-parameter TEXT     CloudFormation parameter for Key
+  --help                   Show this message and exit.
+```
+
+### build-lambda
+
+```
+Usage: stackmanager build-lambda [OPTIONS]
+
+  Build a Lambda function zip file. Can be chained into the upload command
+  where it pre-populates the --filename option.
+
+Options:
+  -s, --source-dir TEXT  Source directory  [required]
+  -o, --output-dir TEXT  Output directory  [required]
+  --runtime TEXT         Lambda Runtime  [required]
+  --archive-name TEXT    Override archive name (defaults to source directory name)
+  --help                 Show this message and exit.
+```
+
+## CI/CD Pipeline support
+
+### Azure DevOps
+
+Stackmanager will automatically detect when it is running in an Azure DevOps pipeline by looking for the 
+`SYSTEM_TEAMPROJECTID` environment variable.
+
+It will print `##vso` strings under the following circumstances:
+
+* `deploy` has created a ChangeSet and it has not been auto-applied: \
+  Sets two variables for the ChangeSet name and identifier. These default to `change_set_name` and `change_set_id`
+  _(since 0.7.0)_ but the name of these variables can be changed with the `CHANGE_SET_NAME_VARIABLE` and 
+  `CHANGE_SET_ID_VARIABLE` environment variables. These values can be used with the `apply` command in a later stage.
+* `deploy` has created a ChangeSet but it contains no changes:\
+   This logs a warning (`##vso[task.logissue]`) and sets the status to `SucceededWithIssues` (`##vso[task.complete]`)
+   allowing following steps/jobs/stages to be skipped by checking for the `SucceededStatus` in a condition.
+* `deploy` or `apply` fails when applying a ChangeSet: \
+   This logs an error (`##vso[task.logissue]`)
+
+## Additional Configuration
+
+> Future plans are to have a global configuration or a larger set of environment variables that can configure
+> behavior.
+
+By default displayed timestamps (e.g. for CloudFormation events) will be displayed in the detected local timezone
+including the timezone offset. If you specify a timezone using the `STACKMANAGER_TIMEZONE` environment variable
+then this will be used instead and the timezone offset will be omitted. Olson Timezones (e.g. America/New_York)
+are supported.
```

