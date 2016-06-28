.. Copyright 2016 FUJITSU LIMITED

.. _applianceImportStatus-get:

applianceImportStatus_get
-------------------------

.. function:: GET /users/{uid}/imports/{iid}/status

.. sidebar:: Summary

	* Method: ``GET``
	* Response Code: ``200 / 304``
	* Response Formats: ``application/xml`` ``application/json``
	* Since: ``UForge 3.5``

Retrieve the current status of importing an appliance archive.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``appliance_create``

URI Parameters
~~~~~~~~~~~~~~

* ``uid`` (required): the id of the :ref:`user-object`
* ``iid`` (required): the id of the :ref:`applianceimport-object` ticket

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "/users/{uid}/imports/{iid}/status" -X GET \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`appliance-object`
	 * :ref:`applianceimport-object`
	 * :ref:`appliance-import`
	 * :ref:`applianceImport-get`
	 * :ref:`applianceImport-upload`
