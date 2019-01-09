---
layout: page
title: Community
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

# Committer Notes

## How To Merge Pull Requests

ref: https://cwiki.apache.org/confluence/pages/viewpage.action?pageId=65865114

The following example is merging Pull-Request-9 to develop branch.

```bash
# Project Setup from Gitbox
git clone https://gitbox.apache.org/repos/asf/incubator-marvin.git
cd incubator-marvin
git remote add mirror https://github.com/apache/incubator-marvin.git

# Update Branch
git checkout develop
git pull origin develop

# Merge Pull Request to Gitbox
git fetch mirror pull/9/head:pr-9
git merge pr-9
git push origin develop
git branch -d pr-9
```

----

* [Community](/marvin-platform-book/ch7_community/overview)
