==========================
Settings
==========================


Redirect to the login page
==========================

Instead of getting a Forbidden (403) error when the user has no permission, you can make the request be redirected to the login page.
Add the following variable to your django ``settings.py``:

``settings.py``

.. code-block:: python

    ROLEPERMISSIONS_REDIRECT_TO_LOGIN = True


.. _register-user-admin-setting:

Regiser User Admin
==================

Replaces the default ``django.contrib.auth.admin.UserAdmin`` with :ref:`RolePermissionsUserAdmin <rolepermissions-useradmin>`
so you can manange roles interactively via the Django User Admin Site.

Add the following variable to your django ``settings.py``:

``settings.py``

.. code-block:: python

    ROLEPERMISSIONS_REGISTER_ADMIN = True
