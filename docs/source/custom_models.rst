Custom Models
=============

You can create your own permission models by extending Django Object Safety's abstract models.

Create a custom ObjectPermission model
--------------------------------------

Import the abstract model and create a new model that inherits from it.

.. code-block:: python

        from django.db import models
        from django_object_safety.models import AbstractObjectPermission

        class MyObjectPermission(AbstractObjectPermission):
            pass

        class Meta:
            app_label = 'my_app'

Next, either add object_permission_model to your model Meta class or set SAFETY_OBJECT_PERMISSION_MODEL setting
in your settings.py:

.. code-block:: python

        class MyModel(models.Model):
            class Meta:
                object_permission_model = MyObjectPermission

or

.. code-block:: python

        SAFETY_OBJECT_PERMISSION_MODEL = 'my_app.MyObjectPermission'