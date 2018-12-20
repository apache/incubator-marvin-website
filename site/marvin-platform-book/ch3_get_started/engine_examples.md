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

# Running a example engine 
1. Clone example engine from repository
```
git clone https://github.com/marvin-ai/engines.git
```
2. Generate a new marvin engine environment for Iris species engine
```
workon python-toolbox-env
marvin engine-generateenv ../engines/iris-species-engine/
```
3. Run the Iris species engine
```
workon iris-species-engine-env
marvin engine-dryrun 
```

For more examples: https://github.com/apache/incubator-marvin/tree/master/public-engines