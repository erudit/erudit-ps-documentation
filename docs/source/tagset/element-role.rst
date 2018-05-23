.. _element-role:

<role>
======

+----------------------------------+--------------------+
| Appears in                       | Frequency          |
+==================================+====================+
| :ref:`element-collab`            | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-contrib`           | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-contrib-group`     | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-element-citation`  | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-person-group`      | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-product`           | Zero or more times |
+----------------------------------+--------------------+

``<role>`` (either function or role) is used to specify an article contributor’s responsibility or function.

Examples:

    * :ref:`element-role-example-1`
    * :ref:`element-role-example-2`

.. _element-role-example-1:

Example of ``<role>`` in ``<contrib>``:
---------------------------------------

.. code-block:: xml

  ...
  <contrib-group content-type="author">
    ...
    <contrib contrib-type="person">
      <contrib-id contrib-id-type="orcid">0000-0003-2125-060X</contrib-id>
      <name>
        <surname>Einstein</surname>
        <given-names>Albert</given-names>
      </name>
      <email>albert@einstein.org</email>
      <role>researcher</role>
      <xref ref-type="aff" rid="aff1"/>
    </contrib>
    ...
  </contrib-group>
  ...

.. _element-role-example-2:

Exemplo de ``<role>`` em ``<element-citation>``:
------------------------------------------------

.. code-block:: xml

    ...
    <element-citation publication-type="journal">
        ...
        <person-group person-group-type="author">
            <name>
                <surname>Petitti</surname>
                <given-names>DB</given-names>
                ...
            </name>
            <name>
                <surname>Crooks</surname>
                <given-names>VC</given-names>
                ...
            </name>
            <role>pesquisador</role>
            ...
        </person-group>
        ...
    </element-citation>
    ...

.. {"reviewed_on": "20180523", "by": "fabio.batalha@erudit.org"}