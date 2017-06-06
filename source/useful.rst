Documentation for the useful
*****************************

.. automodule:: Example

useful #1 -- auto members
=========================

This is something I want to say that is not in the docstring.

.. automodule:: Example.useful
   :members:

useful #2 -- explicit members
=============================

This is something I want to say that is not in the docstring.

.. automodule:: Example.useful
   :members: public_fn_with_sphinxy_docstring, _private_fn_with_docstring

.. autoclass:: MyPublicClass
   :members: get_foobar, _get_baz
