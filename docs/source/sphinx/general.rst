============
Setup Sphinx
============

For a simple setup, check out `this link`_.
To see a list of how to use .rst sytax, check here_.

.. _this link: https://docs.readthedocs.io/en/stable/intro/getting-started-with-sphinx.html
.. _here: https://docutils.sourceforge.io/docs/user/rst/quickref.html

Title
=====

Titles are underlined.
Each new underline-character creates a new subtitle.

You can use the following order: ``= - ~ # * _ +``.
The underline must be at least as long as the title text.
A lone top-level line is lifted up to be the document's title.
Over- and underline creates a higher title level.

.. code:: rst
    
    Title
    =====

    Subtitle
    --------

Bullet lists
============

- Bullets are ``-``, ``*`` or ``+``.
- Continuing text must be aligned
  after the bullet and whitespace.
- Note that a blank line is required before the first item and after the least

Code
----
.. code:: rst

    - Line 1
    - Line 2

    * Line 1
    * Line 2

Output
------
- Line 1
- Line 2

* Line 1
* Line 2

Enumerated lists
================

Enumerators are numbers ``1, 2, ...``, single letters ``a/A, b/B, ...`` or roman numerals ``I, II, ...``.
List items should be sequentially numbered, but **dont need** to start at 1 (although not all formatters will honour the first index).
The ``#`` character will auto-enumerate the item.

Code
----
.. code:: rst

    1. Line
    2. Line
       Multiline
    #. Line

    a. Line
    b. Line

Output
------
1. Line
2. Line
   Multiline
#. Line

a. Line
b. Line