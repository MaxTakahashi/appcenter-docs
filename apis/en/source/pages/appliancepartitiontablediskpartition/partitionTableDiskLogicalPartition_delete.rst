.. Copyright 2016 FUJITSU LIMITED

.. _partitionTableDiskLogicalPartition-delete:

partitionTableDiskLogicalPartition_delete
-----------------------------------------

.. function:: DELETE users/{uid}/appliances/{aid}/installProfile/{ipid}/pt/{ptid}/disks/{did}/partitions/{pid}/lpartitions/{lpid}

.. sidebar:: Summary

	* Method: ``DELETE``
	* Response Code: ``204 / 200``
	* Response Formats: 
	* Since: ``UForge 2.1``

Removes a logical partition from a physical partition.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``appliance_create``

URI Parameters
~~~~~~~~~~~~~~

* ``uid`` (required): the user name (login name) of the :ref:`user-object` that has created the appliance
* ``pid`` (required): the id of the :ref:`partition-object`
* ``ptid`` (required): the id of the :ref:`partitiontable-object`
* ``aid`` (required): the id of the :ref:`appliance-object`
* ``lpid`` (required): the id of the logical :ref:`partition-object`
* ``did`` (required): the id of the :ref:`disk-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

None

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "https://uforge.example.com/apiusers/{uid}/appliances/{aid}/installProfile/{ipid}/pt/{ptid}/disks/{did}/partitions/{pid}/lpartitions/{lpid}" -X DELETE \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml"

.. seealso::

	 * :ref:`appliancepartitiontablediskpartition-api-resources`
	 * :ref:`appliancepartitiontablelogicalgroup-api-resources`
	 * :ref:`appliancepartitiontablelogicalvolume-api-resources`
	 * :ref:`partitiontable-object`
	 * :ref:`appliance-object`
	 * :ref:`partition-object`
	 * :ref:`partitionTableDiskPartition-getAll`
	 * :ref:`partitionTableDiskPartition-get`
	 * :ref:`partitionTableDiskPartition-create`
	 * :ref:`partitionTableDiskPartition-deleteAll`
	 * :ref:`partitionTableDiskPartition-delete`
	 * :ref:`partitionTableDiskPartition-update`
	 * :ref:`partitionTableDiskLogicalPartition-getAll`
	 * :ref:`partitionTableDiskLogicalPartition-get`
	 * :ref:`partitionTableDiskLogicalPartition-create`
	 * :ref:`partitionTableDiskLogicalPartition-deleteAll`
	 * :ref:`partitionTableDiskLogicalPartition-update`
