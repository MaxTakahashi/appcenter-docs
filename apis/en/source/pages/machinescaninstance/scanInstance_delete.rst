.. Copyright 2016 FUJITSU LIMITED

.. _scanInstance-delete:

scanInstance_delete
-------------------

.. function:: DELETE /users/{uid}/scannedinstances/{siid}

.. sidebar:: Summary

	* Method: ``DELETE``
	* Response Code: ``204 / 200``
	* Response Formats: 
	* Since: ``UForge 3.4``

Remove a scanned instance. 

.. warning:: this deletes all the child scan reports and overlay files under this scanned instance.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``migration_access``

URI Parameters
~~~~~~~~~~~~~~

* ``uid`` (required): the user name (login name) of the :ref:`user-object`
* ``siid`` (required): the id of the :ref:`scannedinstance-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "https://uforge.example.com/api/users/{uid}/scannedinstances/{siid}" -X DELETE \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`scannedinstance-object`
	 * :ref:`scan-object`
	 * :ref:`machinescan-api-resources`
	 * :ref:`scannedInstanceScan-getAll`
	 * :ref:`scanInstance-getAll`
	 * :ref:`scanInstance-create`
	 * :ref:`scanInstance-get`
	 * :ref:`scanInstance-deleteAll`
