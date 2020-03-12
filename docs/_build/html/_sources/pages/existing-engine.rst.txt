================================
Working in an Existent Engine
================================

In this section, there are some examples of how to work with an existing engine.

1. If you don’t have an engine locally, clone one to your local machine

2. On Python Toolbox environment, set VirtualEnv and get to engine’s path::

    $ marvin engine-generateenv /path/to/engine/
    $ workon <engine_name>-env


3. Test your engine::

    $ marvin


4. Bring up the notebook and access it from your browser::

    $ marvin notebook


Running a example engine
-----------------------------

1. Clone example engine from repository::

    $ git clone https://github.com/apache/incubator-marvin

2. Generate a new marvin engine environment for Iris species engine::

    $ workon python-toolbox-env
    $ marvin engine-generateenv ../engines/iris-species-engine/

3. Run the Iris species engine::

    $ workon iris-species-engine-env
    $ marvin engine-dryrun

For more examples, access here_. 

.. _here: https://github.com/apache/incubator-marvin/tree/develop/public-engines
