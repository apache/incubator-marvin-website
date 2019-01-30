---
layout: page
title: Architecture
description: Architecture
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

# Architecture

## Design Goal

1. Language Agnostic capabilities: The platform must be able to support R, Python and Scala algorithms
2. Parallelism capacities in many different levels (Eg. GPU, Multi-core and Multi-node) 
3. Deploy distributed machine learning models that are able to receive high concurrent traffic and provide response in near real-time

## Platform Concept Map (High Level Integration)

![concept map](/assets/architecture/concept-map.png)

----

## Quality Attributes

![quality attributes](/assets/architecture/quality-attributes.png)

----

## Architectural Tactics

![architectural tactics](/assets/architecture/architectural-tactics.png)

----

## DASFE

![dasfe](/assets/architecture/dasfe.png)

More Detail in [DASFE](/marvin-platform-book/ch1_main_components/dasfe)

----

## Context Diagram

![context diagram](/assets/architecture/context-diagram.png)

----

## Execution Flow

![execution flow](/assets/architecture/execution-flow.png)

----

## Executor and Engine

![executor engine](/assets/architecture/executor-engine.png)

----

## Cluster Admin

![cluster admin](/assets/architecture/cluster-admin.png)

----

## Deployment Diagram

![deployment diagram](/assets/architecture/deployment-diagram.png)

----

[BACK TO SUMMARY](/marvin-platform-book/SUMMARY)
