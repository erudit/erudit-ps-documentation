.. _element-element-citation:

<element-citation>
==================

Mandatory attributes:

  1. ``@publication-type``

+---------------------+------------+
| Appears in          | Frequency  |
+=====================+============+
| :ref:`element-ref`  | Once       |
+---------------------+------------+




``<element-citation>`` is used to provide a detailed identification of each bibliographic reference, and should only appear as a child of :ref:`element-ref`. In addition, it should have the attribute ``@publication-type`` which indicates the type of the publication of the reference.

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

Examples:

  * :ref:`element-element-citation-example-1`
  * :ref:`element-element-citation-example-2`
  * :ref:`element-element-citation-example-3`

.. _element-element-citation-example-1:

1. Journal
----------

.. code-block:: xml

    <!-- Journal Sample -->

    ...
    <ref-list>
      <ref id="B1">
        <element-citation publication-type="journal">
          <styled-content specific-use="display">
            Arrighi, L. et Boudreau, A. (2013). La construction discursive de l'identité francophone en Acadie ou «comment être francophone à partir des marges?». Minorités linguistiques et société/Linguistic Minorities and Society. 2. 8-92.
          </styled-content>
          <pub-id pub-id-type="doi">
            https://doi.org/10.7202/1016689ar
          </pub-id>           
        </element-citation>
      </ref>
    <ref-list>
    ...


.. _element-element-citation-example-2:

2. Capítulo de livro
--------------------

.. code-block:: xml

    <!-- Book Chapter Sample -->

    ...
    <ref-list>
      <ref id="B1">
        <element-citation publication-type="chapter">
          <styled-content specific-use="display">
            Blommaert, J. et Verschueren, J. (1998). The role of language in European nationalist ideologies. In Schieffelin, B., Woolard, K. et Kroskrity, P. (dir.). Language Ideologies : Practice and Theory. Oxford : Oxford University Press. 189-210.
          </styled-content>
        </element-citation>
      </ref>
    </ref-list>
    ...


.. _element-element-citation-example-3:

3. Livro
--------

.. code-block:: xml

    <!-- Book Sample -->

    ...
    <ref-list>
      <ref id="B1">
        <element-citation publication-type="book">
          <styled-content specific-use="display">
            Baugh, J. (2000). Beyond Ebonics : Linguistic Pride and RacialPrejudice. Oxford : Oxford University Press.
          </styled-content>
        </element-citation>
      </ref>
    </ref-list>
    ...

.. {"reviewed_on": "20180501", "by": "fabio.batalha@erudit.org"}