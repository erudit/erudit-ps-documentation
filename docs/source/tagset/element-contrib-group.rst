.. _element-contrib-group:

<contrib-group>
===============

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+

Contains the group of elements related to the contributions in the drafting of the article. The most frequent contributors are personal authors, institutions and research groups.

Example:

.. code-block:: xml

    ...
    <article-meta>
      ...
      <contrib-group>
        <contrib>
          <name>
            <surname>Arrighi</surname>
            <given-names>Laurence</given-names>
          </name>
          <xref ref-type="aff" rid="aff1"/>
        </contrib>
        <contrib>
          <name>
            <surname>Violette</surname>
            <given-names>Isabelle</given-names>
          </name>
          <xref ref-type="aff" rid="aff1"/>
        </contrib>
      </contrib-group>
      ...
    </article-meta>
    ...
