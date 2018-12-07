---
layout: page
title: Community Members
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

# Creating a new engine
1. To create a new engine
```
workon python-toolbox-env
marvin engine-generate
```
Respond the interactive prompt and wait for the engine environment preparation, and don't forget to start dev box before if you are using vagrant.

2. Test the new engine
```
workon <new_engine_name>-env
marvin test
```
3. For more informations
```
marvin --help
```
4. Youtube Tutorial

[![Creating first engine](http://img.youtube.com/vi/p7yiLh2uLlQ/0.jpg)](https://www.youtube.com/watch?v=p7yiLh2uLlQ "Creating first engine")
