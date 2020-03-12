============================
Install Apache Marvin-AI
============================

Welcome to Apache Marvin-AI install guide.

**We strongly recommend the utilization of Python 3.6 or any latest version.**

Ubuntu Install
--------------


Toolbox will need some OS dependencies::

    $ sudo apt-get install libsasl2-dev python-pip graphviz dialog swig -y

We strongly recommend the use of VirtualEnv and VirtualEnvWrapper::

    $ sudo pip install --upgrade pip
    $ sudo pip install virtualenvwrapper --ignore-installed six


Spark installation (Optional)::

    $ curl https://d3kbcqa49mib13.cloudfront.net/spark-2.1.1-bin-hadoop2.6.tgz -o /tmp/spark-2.1.1-bin-hadoop2.6.tgz
    $ sudo tar -xf /tmp/spark-2.1.1-bin-hadoop2.6.tgz -C /opt/
    $ sudo ln -s /opt/spark-2.1.1-bin-hadoop2.6 /opt/spark
    $ echo "export SPARK_HOME=/opt/spark" >> $HOME/.bash_profile

If you do not have /opt directory created, before unpacking spark, run::

    $ sudo mkdir /opt

Marvin uses dafault values for these environment variables, but you can customize them (Optional)::


    $ echo "export WORKON_HOME=$HOME/.virtualenvs" >> $HOME/.bash_profile
    $ echo "export MARVIN_HOME=$HOME/marvin" >> $HOME/.bash_profile
    $ echo "export MARVIN_DATA_PATH=$HOME/marvin/data" >> $HOME/.bash_profile
    $ echo "source virtualenvwrapper.sh" >> $HOME/.bash_profile
    $ source ~/.bash_profile

Install python-toolbox::

    $ mkvirtualenv python-toolbox-env
    $ setvirtualenvproject
    $ pip install marvin-python-toolbox

Test the installation::

    $ marvin

MacOS Install
--------------


Toolbox will need some OS dependencies::

    $ sudo easy_install pip
    $ brew install openssl graphviz

We strongly recommend the use of VirtualEnv and VirtualEnvWrapper::

    $ sudo pip install --upgrade pip
    $ sudo pip install virtualenvwrapper --ignore-installed six


Spark installation (Optional)::

    $ curl https://d3kbcqa49mib13.cloudfront.net/spark-2.1.1-bin-hadoop2.6.tgz -o /tmp/spark-2.1.1-bin-hadoop2.6.tgz
    $ sudo tar -xf /tmp/spark-2.1.1-bin-hadoop2.6.tgz -C /opt/
    $ sudo ln -s /opt/spark-2.1.1-bin-hadoop2.6 /opt/spark
    $ echo "export SPARK_HOME=/opt/spark" >> $HOME/.bash_profile

If you do not have /opt directory created, before unpacking spark, run::

    $ sudo mkdir /opt

Marvin uses dafault values for these environment variables, but you can customize them (Optional)::


    $ echo "export WORKON_HOME=$HOME/.virtualenvs" >> $HOME/.bash_profile
    $ echo "export MARVIN_HOME=$HOME/marvin" >> $HOME/.bash_profile
    $ echo "export MARVIN_DATA_PATH=$HOME/marvin/data" >> $HOME/.bash_profile
    $ echo "source virtualenvwrapper.sh" >> $HOME/.bash_profile
    $ source ~/.bash_profile

Install python-toolbox::

    $ mkvirtualenv python-toolbox-env
    $ setvirtualenvproject
    $ pip install marvin-python-toolbox

Test the installation::

    $ marvin

Docker Install
--------------
