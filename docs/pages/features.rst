============================
Features
============================

In this section, we show and explain the features of Apache Marvin-AI.

Toolbox CLI
--------------

Here is shown the command line interface (CLI) of the Toolbox.

Usage: marvin [OPTIONS] COMMAND [ARGS]

Options::

      --debug       #Enable debug mode.
      --version     #Show the version and exit.
      --help        #Show this command line interface and exit.

Commands::

      engine-generate     #Generate a new marvin engine project and install...
      engine-generateenv  #Generate a new marvin engine environment and install...
      hive-dataimport     #Export and import data samples from a hive databse to...
      hive-generateconf   #Generate default configuration file
      hive-resetremote    #Drop all remote tables from informed engine on host

Examples::

    $ marvin --help
    $ marvin --version
    $ marvin engine-generate
    $ marvin engine-generateenv .

Engine CLI
--------------

Here is shown the command line interface (CLI) of the Engine.

Usage: marvin [OPTIONS] COMMAND [ARGS]

Options::

      --debug       #Enable debug mode.
      --version     #Show the version and exit.
      --help        #Show this command line interface and exit.

Commands::

      engine-deploy             #Engine provisioning and deployment command
      engine-dryrun             #Marvin Dryrun Utility - Run marvin engines in a...
      engine-grpcserver         #Marvin gRPC engine action server starts
      engine-httpserver         #Marvin http api server starts
      engine-httpserver-remote  #Remote HTTP server control command
      hive-dataimport           #Export and import data samples from a hive...
      hive-generateconf         #Generate default configuration file
      hive-resetremote          #Drop all remote tables from informed engine on...
      lab                       #Start the JupyterLab server.
      notebook                  #Start the Jupyter notebook server.
      pkg-bumpversion           #Bump the package version.
      pkg-createtag             #Create git tag using the package version.
      pkg-showchanges           #Show the package changelog.
      pkg-showinfo              #Show information about the package.
      pkg-showversion           #Show the package version.
      pkg-updatedeps            #Update requirements.txt.
      test                      #Run tests.
      test-checkpep8            #Check python code style.
      test-tdd                  #Watch for changes to run tests automatically.
      test-tox                  #Run tests using a new virtualenv.

Examples::

    $ marvin --help
    $ marvin --version
    $ marvin notebook
    $ marvin engine-dryrun

Setting Environmental Variables
----------------------------------

.. raw:: html

    <style> .red {color:red} </style>

.. role:: red

To set up environmental parameters or variables on Marvin it’s recommended to use the argument :red:`params` that is present on every engine actions.

Setting up params
~~~~~~~~~~~~~~~~~~

You may edit the file *engine.params* that is located at the root directory of your engine. You must insert params as a dictionary::

    {
        "login" : "marvin",
        "password": "123455"
    }

Loading params
~~~~~~~~~~~~~~~~~

Params are loaded as an argument on your engine execution. Then, inside your code you must do :red:`params.get("login")` or :red:`params["login"]` to access those variables.

Samples
~~~~~~~~

* `Example of engine.params file`_
* `Example of loading params on Acquisitor and Cleaner`_

**Notice that if you are running your actions using an API, you may alse set params at the the API body. These params will overwrite the *engine.params* file.**

.. _Example of engine.params file: https://github.com/marvin-ai/marvin-public-engines/blob/master/iris-species-engine/engine.params
.. _Example of loading params on Acquisitor and Cleaner: https://github.com/marvin-ai/marvin-public-engines/blob/master/iris-species-engine/marvin_iris_species_engine/data_handler/acquisitor_and_cleaner.py


