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
| researchid | Identifies a researcher in  *Thomson Reuters*.        |
+------------+-------------------------------------------------------+
| scopus     | Identifies a researcher in  *Scopus*.                 |
+------------+-------------------------------------------------------+

Example:

.. code-block:: xml

  ...
  <contrib-group>
    <contrib contrib-type="author">
      <contrib-id contrib-id-type="orcid">0000-0001-8528-2091</contrib-id>
      <name>
        <surname>Einstein</surname>
        <given-names>Albert</given-names>
      </name>
      ...
    </contrib>
    ...
  </contrib-group>
  ...

.. note:: 

  The element ``<contrib-id>`` can not have URI (URL) data, **it will not be accepted**:

  * ``<contrib-id contrib-id-type="orcid">http://orcid.org/0000-0001-8528-2091</contrib-id>``


.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}
