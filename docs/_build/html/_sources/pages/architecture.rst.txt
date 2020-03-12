============================
Architecture
============================

In this section, we explain the architecture of Apache Marvin-AI. The platform has some specific features, such as:

1. Language Agnostic capabilities: The platform must be able to support R, Python and Scala algorithms
2. Parallelism capacities in many different levels (Eg. GPU, Multi-core and Multi-node)
3. Deploy distributed machine learning models that are able to receive high concurrent traffic and provide response in near real-time

Platform Concept Map (High Level Integration)
-----------------------------------------------

.. image:: ../images/concept-map.png


Quality Attributes
-----------------------

For Data Scientists:
~~~~~~~~~~~~~~~~~~~~~~~~~

 * **Interoperability:** To support different programmer languages 
 * **Usability:** To accelerate and simplify the model creation process

For Administrators:
~~~~~~~~~~~~~~~~~~~~~~~~~

 * **Manageability:** To simplify the distributed deploy/management process 
 * **Usability:** To support from tiny to intensive loads

For Marvin Developers:
~~~~~~~~~~~~~~~~~~~~~~~~~

 * **Modifiability:** To improve and release new versions constantly 
 * **Maintainability:** To allow all type of programmers (from beginners to experts) to contribute


Architectural Tactics
----------------------------

.. image:: ../images/architectural-tactics.png

DASFE
----------------------------

.. image:: ../images/dasfe.png

More details in :ref:`dasfe`.

Context Diagram
----------------------------

.. image:: ../images/context-diagram.png

Execution Flow
----------------------------

.. image:: ../images/execution-flow.png

Executor and Engine
----------------------------

.. image:: ../images/executor-engine.png

Cluster Admin
----------------------------

.. image:: ../images/cluster-admin.png

Deployment Diagram
----------------------------

.. image:: ../images/deployment-diagram.png

