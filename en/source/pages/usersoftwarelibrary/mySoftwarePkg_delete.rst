.. Copyright 2016 FUJITSU LIMITED

.. _mySoftwarePkg-delete:

mySoftwarePkg_delete
--------------------

.. function:: DELETE /users/{uid}/mysoftware/{msid}/pkgs/{mspackid}

.. sidebar:: Summary

	* Method: ``DELETE``
	* Response Code: ``204 / 200``
	* Response Formats: 
	* Since: ``UForge 1.0``

Removes a package binary from a software component. 

.. note:: This does not delete the package meta-data from the software component, only the binary that has been uploaded.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``software_upload``

URI Parameters
~~~~~~~~~~~~~~

* ``uid`` (required): the user name (login name) of the :ref:`user-object`
* ``msid`` (required): the id of the :ref:`mysoftware-object`
* ``mspackid`` (required): the id of the package

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "https://uforge.example.com/api/users/{uid}/mysoftware/{msid}/pkgs/{mspackid}" -X DELETE \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`mysoftware-object`
	 * :ref:`mySoftware-create`
	 * :ref:`mySoftware-getAll`
	 * :ref:`mySoftware-get`
	 * :ref:`mySoftware-update`
	 * :ref:`mySoftware-delete`
	 * :ref:`mySoftwareUsage-getAll`
	 * :ref:`mySoftwarePkg-add`
	 * :ref:`mySoftwarePkg-getAll`
	 * :ref:`mySoftwarePkg-deleteAll`
	 * :ref:`mySoftwarePkg-get`
	 * :ref:`mySoftwarePkg-update`
	 * :ref:`mySoftwarePkg-download`
	 * :ref:`mySoftwarePkg-downloadFile`
	 * :ref:`mySoftwarePkg-upload`
