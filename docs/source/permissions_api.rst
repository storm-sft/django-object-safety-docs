Permissions API
===============

Setting a permission
--------------------

Import set_perm:

.. code-block:: python

   from safety.shortcuts import set_perm

Set an object permission:

.. code-block:: python

   set_perm([user_or_group], 'view_post', obj)
Set a global permission:

.. code-block:: python

   set_perm([user_or_group], 'view_post', content_type=contentTypeOfModel)


Lifting a permission
--------------------

Import lift_perm:

.. code-block:: python

   from safety.shortcuts import lift_perm
Lift (remove) an object permission:

.. code-block:: python

   lift_perm([user_or_group], 'view_post', obj)
Lift (remove) a global permission:

.. code-block:: python

   lift_perm([user_or_group], 'view_post', content_type=contentTypeOfModel)


Checking a permission
---------------------

Import has_perm:

.. code-block:: python

   from safety.shortcuts import has_perm
Check an object permission:

.. code-block:: python

   has_perm([user_or_group], 'view_post', obj)
Check a global permission:

.. code-block:: python

   has_perm([user_or_group], 'view_post', content_type=contentTypeOfModel)


Checking a permission (including group permissions)
---------------------------------------------------

Import the shortcut:

.. code-block:: python

   from safety.shortcuts import has_gross_perm

Check if a user has permission to an object group, group, or directly:

.. code-block:: python

   has_gross_perm([user], 'permission_codename', obj)

Get an object permission
------------------------

Import the shortcut:

.. code-block:: python

   from safety.shortcuts import get_object_perm

Get an object permission:

.. code-block:: python

   get_object_perm([user], 'permission_codename', obj)

Get users with permissions
--------------------------

Import the shortcut:

.. code-block:: python

   from safety.shortcuts import get_users_with_perms

Get users with permissions:

.. code-block:: python

   get_users_with_perms('permission_codename', obj)

Get users with gross permissions (includes permissions through groups)
----------------------------------------------------------------------

Import the shortcut:

.. code-block:: python

   from safety.shortcuts import get_users_with_perms

Get users with permissions:

.. code-block:: python

   get_users_with_perms('permission_codename', obj, with_group_users=True)

Get groups with permissions
---------------------------

Import the shortcut:

.. code-block:: python

   from safety.shortcuts import get_groups_with_perms

Get groups with permissions (obj can be None, it's default value):

.. code-block:: python

   get_groups_with_perms('permission_codename', obj)
