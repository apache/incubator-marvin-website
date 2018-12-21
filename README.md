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

# Apache Marvin-AI

This project is the document and website of Apache Marvin-AI.

This template was generated using [Jekyll](https://jekyllrb.com/),
based on [Apache Website Template](https://github.com/apache/apache-website-template)

# How to setup the web site locally

## Setup

```
1. cd site
3. sudo apt-get install rubygems ruby2.1-dev zlib1g-dev
4. sudo gem install bundler github-pages jekyll
5. bundle install
```

## Running locally

Before opening a pull request, you can preview your contributions by
running from within the directory:

```
1. bundle exec jekyll serve
2. Open [http://localhost:4000](http://localhost:4000)
```

## Adding contributors

To add a contributor to the project, or to modify existing contributors,
edit `site/_data/contributors.yml`.
The [project members]([http://localhost:4000/community.html#project-members])
list will re-generate.
