.. _element-contrib-id:

<contrib-id>
============

Mandatory attributes:

  1. ``@contrib-id-type``

+-------------------------+--------------------+
| Appears in              | Frequency          |
+=========================+====================+
| :ref:`element-contrib`  | Zero or more times |
+-------------------------+--------------------+

This is the digital identifier of the researcher.

The attribute ``@contrib-id-type`` could have the following values:

+------------+-------------------------------------------------------+
|  Value     | Description                                           |
+============+=======================================================+
| orcid      | Identifies a researcher in  *ORCID Organization*.     |
+------------+-------------------------------------------------------+
| isns       | Identifies a researcher in  *ISNI*.                   |
+------------+-------------------------------------------------------+

Example:

.. code-block:: xml

  ...
  <contrib-group>
    <contrib contrib-type="author">
      <contrib-id contrib-id-type="orcid">0000-0001-8528-2091</contrib-id>
      <name>
        <surname>Brown</surname>
        <given-names>Emmett</given-names>
      </name>
      ...
    </contrib>
    ...
  </contrib-group>
  ...

.. code-block:: xml

  ...
  <contrib-group>
    <contrib contrib-type="author">
      <contrib-id contrib-id-type="isns"></contrib-id>
      <name>
        <surname>Brown</surname>
        <given-names>Emmett</given-names>
      </name>
      ...
    </contrib>
    ...
  </contrib-group>
  ...

.. note:: 

  The element ``<contrib-id>`` can not have URI (URL) data, **it will not be accepted**:

  * ``<contrib-id contrib-id-type="orcid">http://orcid.org/0000-0001-8528-2091</contrib-id>``


.. {"reviewed_on": "20190411", "by": "fabio.batalha@erudit.org"}
