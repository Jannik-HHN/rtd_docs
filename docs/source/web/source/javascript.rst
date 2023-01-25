============
JavaScript
============

Get a specific HTML element by id

.. code:: javascript

    var element = document.getElementById("id-1")

----

Get all HTML elements by a specific class name

.. code:: javascript
    
    var elements = document.getElementsByClassName("class-name")
    // Only select first element in array
    var element = document.getElementsByClassName("class-name")[0]

----

Add or remove a single or multiple classes to an element.

.. code:: javascript

    element.classList.add("class-1", "class-2")
    element.classList.remove("class-1", "class-2")

----

Set style attributes for an element

.. code:: javascript
    
    element.style.display = "flex"

----

Set children elements or content for an element

.. code:: javascript

    // Override current children
    element.innerHTML = "Hello World"
    // Append to current children
    element.innerHTML += 
        '<div class="class-1">' +
            '<p>Goodbye</p>'    +
        '</div>'

----

Execute code line after a set amount of milliseconds

.. code:: javascript

    setTimeout(() => {
        console.log("Timer timed out")
    }, 1000);

----

Create a random number between 0 and 1. In this case if its multiplied by 6 the numbers can range from 0-5.

.. code:: javascript
    
    var range = 6
    var random_number = Math.floor((Math.random() * range))