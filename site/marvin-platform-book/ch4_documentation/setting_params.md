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

# Setting Environmental Variables

To set up environmental parameters or variables on Marvin it's recommended 
to use the argument ```params``` that is present on every engine actions.

## Setting up params
You may edit the file *engine.params* that is located at the root directory 
of your engine. You must insert params as a dictionary:

```json
{
    "login" : "marvin",
    "password": "123455"
}
```

## Loading params
Params are loaded as an argument on your engine execution. Then, inside your 
code you must do ```params.get("login")``` or ```params["login"]``` to access 
those variables.

## Samples
* [Example of *engine.params* file](https://github.com/marvin-ai/marvin-public-engines/blob/master/iris-species-engine/engine.params)
* [Example of loading params on **Acquisitor and Cleaner**](https://github.com/marvin-ai/marvin-public-engines/blob/master/iris-species-engine/marvin_iris_species_engine/data_handler/acquisitor_and_cleaner.py)

**Notice that  if you are running your actions using an API, you may alse set params at 
the the API body. These params will overwrite the <i>engine.params</i> file.**

----

* [Documentation](/marvin-platform-book/ch4_documentation/overview)