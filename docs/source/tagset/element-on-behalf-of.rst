.. _element-on-behalf-of:

<on-behalf-of>
==============

+-------------------------------+--------------------+
| Appears in                    | Frequency          |
+===============================+====================+
| :ref:`element-contrib-group`  | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-contrib`        | Zero or more times |
+-------------------------------+--------------------+

Used when the author acts as a representative of a group or organization in the authorship or in the editing of the article..

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
      <xref ref-type="aff" rid="aff1"/>
      <on-behalf-of>Back to the Future Company</on-behalf-of>
      ...
    </contrib>
    ...
  </contrib-group>
  ...


.. {"reviewed_on": "20180524", "by": "fabio.batalha@erudit.org"}
