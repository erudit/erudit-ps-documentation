.. _element-element-citation:

<element-citation>
==================

+---------------------+--------------------+
| Appears in          | Frequency          |
+=====================+====================+
| :ref:`element-ref`  | Zero or once       |
+---------------------+--------------------+

``<element-citation>`` is used to provide a detailed identification of each bibliographic reference, and should only appear as a child of :ref:`element-ref`. In addition, it could have the attribute ``@publication-type`` which indicates the type of the publication of the reference.

``<element-citation>`` is used in :ref:`element-ref` to identify the DOI of the cited article.

.. note:

    For the current version of :term:`Érudit PS`, it is not mandatory to identify the ``@publication-type`` in ``element-citation``, but have in mind in the future this attribute should became mandatory.

The possible values for the ``@publication-type`` attribute are:

+-----------+------------------------------------------------------------------+
| Value     | Description                                                      |
+===========+==================================================================+
| book      | Refers to books. It can also represent only a part or chapter of |
|           | a book.                                                          |
+-----------+------------------------------------------------------------------+
| chapter   | Refers to books. It can also represent only a part or chapter of |
|           | a book.                                                          |
+-----------+------------------------------------------------------------------+
| confproc  | Identifies documents related to scientific events: minutes,      |
|           | annals, results, proceedings, conventions and conferences,       |
|           | among others.                                                    |
+-----------+------------------------------------------------------------------+
| data      | Specifies databases.                                             |
+-----------+------------------------------------------------------------------+
| magazine  | Referencia livros. Pode também representar somente uma parte ou  |
|           | capítulo de um livro.                                            |
+-----------+------------------------------------------------------------------+
| journal   | Characterized by serial publications, edited in successive       |
|           | units / issues, with numerical and / or chronological            |
|           | designations, and destined to be continued indefinitely.         |
+-----------+------------------------------------------------------------------+
| patent    | Refers to patents.                                               |
+-----------+------------------------------------------------------------------+
| report    | Identifies a unique technical report, normally authored by an    |
|           | institution.                                                     |
+-----------+------------------------------------------------------------------+
| software  | Refers to a software distributed on CDs, DVDs, online media, USB |
|           | devices, etc.                                                    |
+-----------+------------------------------------------------------------------+
| thesis    | Characterized by monographs, dissertations or theses to attain an|
|           | academic degree (doctorate, master's, baccalaureate, bachelor's  |
|           | degree, etc.).                                                   |
+-----------+------------------------------------------------------------------+
| webpage   | Identifies web sites e blogs.                                    |
+-----------+------------------------------------------------------------------+
| newspaper | Identifies newspapers articles.                                  |
+-----------+------------------------------------------------------------------+

.. note::

    For compatibility with ``Érudit Article`` see :ref:`compatibility-reference` section.

Examples:

  * :ref:`element-element-citation-example-1`
  * :ref:`element-element-citation-example-2`
  * :ref:`element-element-citation-example-3`

.. _element-element-citation-example-1:

1. Mixed-citation only
----------------------

.. code-block:: xml

    <!-- Journal Sample -->

    ...
    <ref-list>
      <ref id="B1">
        <mixed-citation publication-type="journal">
            Arrighi, L. et Boudreau, A. (2013). La construction discursive de l'identité francophone en Acadie ou «comment être francophone à partir des marges?». Minorités linguistiques et société/Linguistic Minorities and Society. 2. 8-92.
        </mixed-citation>
      </ref>
    <ref-list>
    ...

.. _element-element-citation-example-2:

2. Mixed-citation and element-citation (DOI only)
----------------------

.. code-block:: xml

    <!-- Journal Sample -->

    ...
    <ref-list>
      <ref id="B1">
        <mixed-citation publication-type="journal">
            Arrighi, L. et Boudreau, A. (2013). La construction discursive de l'identité francophone en Acadie ou «comment être francophone à partir des marges?». Minorités linguistiques et société/Linguistic Minorities and Society. 2. 8-92.
        </mixed-citation>
        <element-citation publication-type="journal">
          <pub-id pub-id-type="doi">
              https://doi.org/10.7202/1016689ar
          </pub-id>
        </element-citation>
      </ref>
    <ref-list>
    ...

.. _element-element-citation-example-3:

3. Mixed-citation and  detailed element-citation
------------------------------------------------

.. code-block:: xml

    <!-- Journal Sample -->

    ...
    <ref-list>
      <ref id="B1">
        <mixed-citation publication-type="journal">
            Arrighi, L. et Boudreau, A. (2013). La construction discursive de l'identité francophone en Acadie ou «comment être francophone à partir des marges?». Minorités linguistiques et société/Linguistic Minorities and Society. 2. 8-92.
        </mixed-citation>
        <element-citation publication-type="journal">
        <person-group person-group-type="author">
            <name>
              <surname>
                  Arrighi
              </surname>
              <given-names>
                  L.
              </given-names>
            </name>
            <name>
              <surname>
                  Boudreau
              </surname>
              <given-names>
                  A.
              </given-names>
            </name>
          </person-group>
          <year>
              2013
          </year>
          <source>
              Minorités linguistiques et société
          </source>
            <article-title>
                La construction discursive de l'identité francophone en Acadie ou «comment être francophone à partir des marges?»
            </article-title>
          <issue>
              2
          </issue>
          <fpage>
              8
          </fpage>
          <lpage>
              92
          </lpage>
          <pub-id pub-id-type="doi">
              https://doi.org/10.7202/1016689ar
          </pub-id>
        </element-citation>
      </ref>
    <ref-list>
    ...







.. {"reviewed_on": "20180501", "by": "fabio.batalha@erudit.org"}
