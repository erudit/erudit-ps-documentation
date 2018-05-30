.. _element-collab:

<collab>
========

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-contrib`       | Zero or more times |
+------------------------------+--------------------+
| :ref:`element-person-group`  | Zero or more times |
+------------------------------+--------------------+

Identifies individual or group institutional authorship.

Examples:

  * :ref:`element-collab-example-1`
  * :ref:`element-collab-example-2`
  * :ref:`element-collab-example-3`


.. _element-collab-example-1:

Example of ``<collab>`` in ``<front>``:
---------------------------------------

.. code-block:: xml

  ...
  <contrib-group>
    <contrib contrib-type="author">
      <collab>
        <named-content content-type="name">The Mouse Genome Sequencing Consortium</named-content>
      </collab>
    </contrib>
    <contrib contrib-type="author">
      <name>
        <surname>Zappi</surname>
        <given-names>Daniela C.</given-names>
      </name>
      <xref ref-type="corresp" rid="c1">1</xref>
    </contrib>
  </contrib-group>
  ...

.. _element-collab-example-2:

Example of ``<collab>`` for groups:
-----------------------------------

.. code-block:: xml

  ...
  <contrib-group content-type="author">
    <contrib contrib-type="person" equal-contrib="yes">
      <name>
        <surname>Church</surname><given-names>Deanna M.</given-names>
      </name>
      <xref ref-type="aff" rid="aff1"/>
    </contrib>
    <!-- NOTE: Group authors are not yet supported by Texture! -->
    <contrib contrib-type="group" equal-contrib="yes">
      <collab>
        <named-content content-type="name">The Mouse Genome Sequencing Consortium</named-content>
        <uri content-type="entity">organisation-25</uri>
        <contrib-group>
          <contrib>
            <name>
              <surname>Kelly</surname><given-names>Laura A.</given-names>
            </name>
          </contrib>
          <contrib>
            <name>
              <surname>Randall</surname><given-names>Daniel Lee</given-names>
              <suffix>Jr.</suffix>
            </name>
          </contrib>
        </contrib-group>
      </collab>
    </contrib>
  </contrib-group>
  ...

.. _element-collab-example-3:

Example of ``<collab>`` in ``<back>``:
--------------------------------------

.. code-block:: xml

    ...
    <element-citation publication-type="book">
      <person-group person-group-type="author">
        <collab>
          <named-content cotent-type="name">World Health Organization (WHO)</named-content>
        </collab>
      </person-group>
      <source>The top 10 causes of death. Fact sheet nº 310</source>
      ...
    </element-citation>
    ...


.. {"reviewed_on": "20180517", "by": "fabio.batalha@erudit.org"}