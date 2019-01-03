---
layout: page
title: Installation
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

# Installing Toolbox using vagrant

1. Install requirements
- [Virtual box](http://www.virtualbox.org) (Version 5.1 +)
- [Vagrant](http://www.vagrantup.com) (Version 1.9.2 or +)


2. Clone repository and start provision

```
git clone https://github.com/marvin-ai/marvin-vagrant-dev.git
cd marvin-vagrant-dev
```

3. Prepare dev (engine creation) box

```
vagrant up dev
vagrant ssh dev
```

Wait for provision process and follow interactive configuration script after access the dev box using vagrant ssh command.

4. The marvin source projects will be on your home folder, to compile and use the marvin toolbox

```
workon python-toolbox-env
make marvin
```

----

* [Installing Marvin](/marvin-platform-book/ch2_toolbox_installation/overview)