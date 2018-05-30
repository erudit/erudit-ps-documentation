.. _element-contrib-group:

<contrib-group>
===============

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+
| :ref:`element-journal-meta`  | Zero or more times |
+------------------------------+--------------------+

Contains the group of elements related to the contributions in the drafting of the article. The most frequent contributors are personal authors, institutions and research groups.

Inside :ref:`element-article-meta`, the attribute ``@content-type`` is not mandatory, but once used the allowed values are:

+----------+
| Value    |
+==========+
| author   |
+----------+
| editor   |
+----------+

Inside :ref:`element-journal-meta`, the attribute ``@content-type`` is not mandatory, but once used the allowed values are:

+----------+
| Value    |
+==========+
| editor   |
+----------+
| manager  |
+----------+

.. note::

  The elements :ref:`element-aff` and :ref:`element-aff-alternatives` are not allowed in ``<contrib-group>``

.. note::

  Some of the refered rules are based on `JATS4M specifications <https://github.com/substance/dar/blob/master/DarArticle.md#contrib-group>`_.

Examples:

 * :ref:`element-label-example-1`
 * :ref:`element-label-example-2`

 .. _element-label-example-1:

Example in ``<article-meta>``:
------------------------------

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

 .. _element-label-example-1:

Example in ``<journal-meta>``:
------------------------------

.. code-block:: xml

    ...
    <journal-meta>
      <contrib-group content-type="manager">
        <contrib contrib-type="person">
          <name>
            <surname>Jolicoeur</surname>
            <given-names>Serge</given-names>
          </name>
          <role>director</role>
        </contrib>
      </contrib-group>
      <contrib-group content-type="editor">
        <contrib contrib-type="person">
          <name>
            <surname>Léger</surname>
            <given-names>Catherine</given-names>
          </name>
          <role>redacteur chef</role>
        </contrib>
        <contrib contrib-type="person">
          <name>
            <surname>LeBlanc</surname>
            <given-names>Matthieu</given-names>
          </name>
          <role>redacteur chef</role>
        </contrib>
        <contrib contrib-type="person">
          <name>
            <surname>Arrighi</surname>
            <given-names>Laurence</given-names>
          </name>
          <role>redacteur chef</role>
        </contrib>
        <contrib contrib-type="person">
          <name>
            <surname>Violette</surname>
            <given-names>Isabelle</given-names>
          </name>
          <role>redacteur chef</role>
        </contrib>
      </contrib-group>
      ...
    </journal-meta>
    ...

.. {"reviewed_on": "20180530", "by": "fabio.batalha@erudit.org"}