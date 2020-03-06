============
EssipLib-doc
============



Build this documentation
========================

With pipenv
-----------
Requirements (system)

* make

Requirements (Python 3):

* pipenv (will automatically download all the project requirements from pypi)
   .. code::shell
      
      pip install --user pipenv

Create a virtual environment with pipenv (will use the Pipfile for installing the necessary packages)

.. code:: shell

   pipenv install

then you can build the documentation

.. code:: shell

   pipenv run make html

The command ..command 

if you want run ``make`` multiple times, prepone ``pipenv run`` on each command can be annoying,
you can spawn a subshell with

.. code:: shell

   pipenv shell

and then you can use ``make`` the usual way

.. code:: shell

   make html     # for html
   make github   # runs make html and copy the result in docs/
   make latex    # for latex
   make latexpdf # for latex (will require latexpdf installed)
   make          # list all the available output format

all the outputs will be in docs folder (for html: docs/html)

