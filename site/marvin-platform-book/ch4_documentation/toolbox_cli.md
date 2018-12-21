---
layout: page
title: Interface
description: Project Community Page
group: nav-right
---
<!--
{% comment %}
Licensed to the Apache Software Foundation (ASF) under one or more
contributor license agreements.  See the NOTICE file distributed with
this work for additional information regarding copyright ownership.
The ASF licenses this file to you under the Apache License, Version 2.0
(the "License"); you may not use this file except in compliance with
the License.  You may obtain a copy of the License at

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
{% endcomment %}
-->

{% include JB/setup %}

# Toolbox CLI

### Command line interface
Usage: marvin [OPTIONS] COMMAND [ARGS]

Options:

```
  --debug       #Enable debug mode.
  --version     #Show the version and exit.
  --help        #Show this command line interface and exit.
```

Commands:

```
  engine-generate     #Generate a new marvin engine project.
  engine-generateenv  #Generate a new marvin engine environment.
  engine-grpcserver   #Marvin gRPC engine action server starts.
  engine-httpserver   #Marvin http api server starts.
  hive-dataimport     #Import data samples from a hive databse to the hive running in this toolbox.
  hive-generateconf   #Generate default configuration file.
  hive-resetremote    #Drop all remote tables from informed engine on host.
  notebook            #Start the Jupyter notebook server.
  pkg-bumpversion     #Bump the package version.
  pkg-createtag       #Create git tag using the package version.
  pkg-showchanges     #Show the package changelog.
  pkg-showinfo        #Show information about the package.
  pkg-showversion     #Show the package version.
  pkg-updatedeps      #Update requirements.txt.
  test                #Run tests.
  test-checkpep8      #Check python code style.
  test-tdd            #Watch for changes to run tests automatically.
  test-tox            #Run tests using a new virtualenv.
```

----

* [Documentation](/marvin-platform-book/ch4_documentation/overview)