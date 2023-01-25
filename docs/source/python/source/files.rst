============
Files
============

Read a single line from a text file

.. code:: python

    with open('file.txt') as file:
        line  = file.readline()
        line2 = file.readline()

.. note:: 
    If the end of a file has been reached, the ``readline()`` returns an empty string

----

Read all the lines of the text file into a list of strings

.. code:: python

    with open('file.txt') as file:
        contents = file.readlines()

----

Read a whole text file into a single string

.. code:: python

    with open('file.txt') as file:
        contents = file.read()

----

Read a text file line by line

.. code:: python

    with open('file.txt') as file:
        for line in file:
            print(line.strip())

.. note:: 
     The ``strip()`` function will remove the newline character ``\n``

----

Read ``.json`` file and load content into a Python ``dict()``

.. code:: python

    with open('file.json', encoding='utf8') as file:
        content = json.load(file)

----

Write JSON content to a file

.. code:: python

    with open('file.json', 'w', encoding='utf8') as file:
        file.write(json.dumps(content, ensure_ascii=False))