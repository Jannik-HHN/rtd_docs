============
Arrays
============

Combine multiple arrays
-----------------------

.. code:: python

    array_main = []

    array_1 = [
        {"key1": "value1"},
        {"key2": "value2"}
    ]

    array_2 = [
        {"key3": "value3"},
        {"key4": "value4"}
    ]
        
    array_main += array_1
    array_main += array_2

.. code:: python

    >> print(array_main)
    [{'key1': 'value1'}, {'key2': 'value2'}, {'key3': 'value3'}, {'key4': 'value4'}]

.. note:: 
    Notice that only the **content of the array** is added and not the array itself!


Append arrays
-----------------------

.. code:: python

    array_main = []

    array_1 = [
        {"key1": "value1"},
        {"key2": "value2"}
    ]

    array_2 = [
        {"key3": "value3"},
        {"key4": "value4"}
    ]
        
    array_main.append(array_1)
    array_main.append(array_2)


.. code:: python

    >> print(array_main)
    [[{'key1': 'value1'}, {'key2': 'value2'}], [{'key3': 'value3'}, {'key4': 'value4'}]]

.. note:: 
    Notice that the **actual array** is added!