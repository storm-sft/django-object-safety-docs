Usage
=====

.. _installation:

Installation
------------

To use Django Object Safety, first install it using pip:

.. code-block:: console

   (.venv) $ pip install django-object-safety

or with poetry:

.. code-block:: console

   (.venv) $ poetry add django-object-safety

Setup
-----

Add safety to your INSTALLED_APPS
.. code-block:: python
   INSTALLED_APPS = [
       ...
       'safety',
       ...
   ]
