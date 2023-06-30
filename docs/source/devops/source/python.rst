============
Python
============

Basic execution for python scripts in Visual Studio Code

.. code:: bash

    # Allow to run scripts in VSC
    Get-ExecutionPolicy -List
    Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser

----

Setup virtual environment

.. code:: bash

    # Creating virtual environment
    python -m venv <env_name>

    # Activate virtual environment
    .venv\scripts\activate

----

Create ``requirements.txt`` file from installed pip packages

.. code:: bash

    # List requirements in console
    python -m pip list
    python -m pip freeze

    # Create requirements file
    python -m pip freeze > requirements.txt

----

Install dependencies

.. code:: bash

    # Install package
    python -m pip install <name>

    # Upgrade package
    python -m pip install --upgrade <name>

    # Install all packages from requirements.txt file
    python -m pip install -r requirements.txt

----

Django specific commands

.. code:: bash

    # Apply changes to database
    python manage.py makemigrations
    python manage.py migrate

    # Run Backend Server
    python manage.py runserver