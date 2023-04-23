Object Group API
================

Creating an object group
------------------------
Import the shortcut:

.. code-block:: python

   from safety.shortcuts import create_object_group

Create an object group:

.. code-block:: python

   create_object_group(name='my-object-name', permissions=['view_modelname', 'change_modelname'], obj)


Deleting an object group:
-------------------------
Import the shortcut:

.. code-block:: python

   from safety.shortcuts import delete_object_group

Delete an object group:

.. code-block:: python

   delete_object_group(name='my-object-name', obj)


Adding a user to an object group:
---------------------------------

Import the shortcut:

.. code-block:: python

   from safety.shortcuts import add_user_to_object_group

Add a user to an object group:

.. code-block:: python

   add_user_to_object_group(user, name='my-object-name', obj)


Removing a user from an object group:
-------------------------------------

Import the shortcut:

.. code-block:: python

   from safety.shortcuts import remove_user_from_object_group

Remove a user from an object group:

.. code-block:: python

   remove_user_from_object_group(user, name='my-object-name', obj)
