tri.table
==========

.. image:: https://travis-ci.org/TriOptima/tri.table.svg?branch=master
    :target: https://travis-ci.org/TriOptima/tri.table


.. image:: https://codecov.io/github/TriOptima/tri.table/coverage.svg?branch=master
    :target: https://codecov.io/github/TriOptima/tri.table?branch=master


tri.table is a library to make full featured HTML tables easily:

* generates header, rows and cells
* grouping of headers
* filtering
* sorting
* bulk edit
* pagination
* automatic rowspan
* link creation
* customization on multiple levels, all the way down to templates for cells

All these examples and a bigger example using many more features can be found in the examples django project.

Read the full documentation for more.

Simple example
--------------

.. literalinclude:: ../examples/examples/views.py
   :pyobject: readme_example_1

And this is what you get:

.. image:: table_example_1.png


Downloading tri.table and running examples
------------------------------------------

.. code-block:: bash

    git clone https://github.com/TriOptima/tri.table.git
    cd tri.table/examples
    virtualenv venv
    source venv/bin/activate
    pip install "django>=1.8,<1.9"
    pip install tri.table
    python manage.py migrate
    python manage.py runserver localhost:8000
    # Now point your browser to localhost:8000 in order to view the examples.


Fancy django features
---------------------

Say I have some models:

.. literalinclude:: ../examples/examples/models.py
   :pyobject: Foo
.. literalinclude:: ../examples/examples/models.py
   :pyobject: Bar

Now I can display a list of Bars in a table like this:

.. literalinclude:: ../examples/examples/views.py
   :pyobject: readme_example_2

This gives me a view with filtering, sorting, bulk edit and pagination.

All these examples and a bigger example using many more features can be found in the examples django project.

Read the full documentation for more.




Running tests
-------------

You need tox installed then just `make test`.


License
-------

BSD


Documentation
-------------

http://tritable.readthedocs.org.
