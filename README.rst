============
 Dictdiffer
============

.. image:: https://travis-ci.org/inveniosoftware/dictdiffer.png?branch=master
    :target: https://travis-ci.org/inveniosoftware/dictdiffer
.. image:: https://coveralls.io/repos/inveniosoftware/dictdiffer/badge.png?branch=master
    :target: https://coveralls.io/r/inveniosoftware/dictdiffer
.. image:: https://pypip.in/v/dictdiffer/badge.png
   :target: https://pypi.python.org/pypi/dictdiffer/
.. image:: https://pypip.in/d/dictdiffer/badge.png
   :target: https://pypi.python.org/pypi/dictdiffer/


About
=====

Dictdiffer is a helper module that helps you to diff and patch
dictionaries.


Fork note
=========

This fork branches off upstream at commit ``18a8b4c`` (January 2015) and changes
one thing: ``diff()`` always returns the path to a changed item as a list of
keys, instead of joining string keys with dots. With keys that contain dots
themselves (``'a.b'``) the dotted path was ambiguous and hard to trace back to
the right place. The version numbers were changed only for an internal package.


Installation
============
Dictdiffer is on PyPI so all you need is: ::

    pip install dictdiffer


Documentation
=============

Documentation is readable at http://dictdiffer.readthedocs.org or can be
built using Sphinx: ::

    pip install dictdiffer[docs]
    python setup.py build_sphinx


Testing
=======
Running the test suite is as simple as: ::

    ./run-tests.sh
