.. Copyright 2016 FUJITSU LIMITED

.. _os-update:

os_update
---------

.. function:: PUT /distributions/{id}

.. sidebar:: Summary

	* Method: ``PUT``
	* Response Code: ``200``
	* Response Formats: ``application/xml`` ``application/json``
	* Since: ``UForge 1.0``

Updates the meta-data information of an operating system. 

Please refer to :ref:`distribprofile-object` for a complete list of all the ``os`` attributes.

Security Summary
~~~~~~~~~~~~~~~~

* Requires Authentication: ``true``
* Entitlements Required: ``org_os_administrate``

URI Parameters
~~~~~~~~~~~~~~

* ``id`` (required): the id of the :ref:`org-object`

HTTP Request Body Parameters
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

A :ref:`distribution-object` object

Example Request
~~~~~~~~~~~~~~~

.. code-block:: bash

	curl "https://uforge.example.com/api/distributions/{id}" -X PUT \
	-u USER_LOGIN:PASSWORD -H "Accept: application/xml" --data-binary "@representation.xml"

Example of representation.xml content (the request body):

.. code-block:: xml

	<ns0:distribution xmlns:ns0="http://www.usharesoft.com/uforge">
		<active>false</active>
	</ns0:distribution>


.. seealso::

	 * :ref:`distribprofile-object`
	 * :ref:`os-create`
	 * :ref:`os-getAll`
	 * :ref:`os-get`
	 * :ref:`osAccess-update`
	 * :ref:`osLicense-download`
	 * :ref:`osLogo-download`
	 * :ref:`osLogo-downloadFile`
	 * :ref:`osPkg-getAll`
	 * :ref:`osPkg-get`
	 * :ref:`osPkgUpdates-getAll`
