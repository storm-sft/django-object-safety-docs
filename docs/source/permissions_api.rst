Permissions API
===========

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
