.. _element-contrib:

<contrib>
=========

+-------------------------------+-------------------+
| Appears in                    | Frequency         |
+===============================+===================+
| :ref:`element-contrib-group`  | One or more times |
+-------------------------------+-------------------+

Identifies individual, institutional or group data of the contributors to the article, who may even be anonymous. The elements :ref:`element-name`, :ref:`element-collab`, :ref:`element-on-behalf-of`, :ref:`element-xref`, :ref:`element-role` and ``<anonymous>`` can be in this element.

The attribute ``@contrib-type`` is not mandatory, it defines the type of contribution and can have the values outlined below:

+------------+----------------------------------------------------------------+
| Value      | Description                                                    |
+============+================================================================+
| person     | Any person involved with the article production                |
+------------+----------------------------------------------------------------+
| group      | Any group of person related to a context, institution,         |
|            | department, etc                                                |
+------------+----------------------------------------------------------------+

.. note::

  When a contrib is defined as **group** it must have an element :ref:`element-collab` inside specifing the name or context of the group. To identify the group it could be made using the element :ref:`element-named-content` with the attribute ``@content-type`` equal **name**.

.. note::

  Some of the refered rules are based on `JATS4M specifications <https://github.com/substance/dar/blob/master/DarArticle.md#contrib-group>`_.

Example:

.. code-block:: xml

  ...
  <article-meta>
    ...
    <contrib-group content-type="author">
      <contrib contrib-type="person">
        <name>
          <surname>Church</surname><given-names>Deanna M.</given-names>
        </name>
        <xref ref-type="aff" rid="aff1"/>
      </contrib>
      <contrib contrib-type="group">
        <collab>
          <named-content content-type="name">The Mouse Genome Sequencing Consortium</named-content>
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
  </article-meta>
  ...

.. {"reviewed_on": "20180516", "by": "fabio.batalha@erudit.org"}