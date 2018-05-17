.. _element-contrib-group:

<contrib-group>
===============

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+

Contains the group of elements related to the contributions in the drafting of the article. The most frequent contributors are personal authors, institutions and research groups.

The attribute ``@content-type`` is not mandatory, but once used the allowed values are:

+----------+
| Value    |
+==========+
| author   |
+----------+
| editor   |
+----------+

.. note::

  The elements :ref:`element-aff` and :ref:`element-aff-alternatives` are not allowed in ``<contrib-group>``

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
            <surname>Arrighi</surname>
            <given-names>Laurence</given-names>
          </name>
          <xref ref-type="aff" rid="aff1"/>
        </contrib>
        <contrib contrib-type="person">
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

.. {"reviewed_on": "20180516", "by": "fabio.batalha@erudit.org"}