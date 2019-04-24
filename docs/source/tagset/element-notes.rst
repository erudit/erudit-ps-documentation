.. _element-notes:

<notes>
======

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-front`         | Zero or one        |
+------------------------------+--------------------+

The element ``<notes>`` is used to identify the editorial notes related to the article, the issue the article is publisher, translations notes, etc.

Examples:

  * :ref:`element-name-example-1`
  * :ref:`element-name-example-2`
  * :ref:`element-name-example-3`

.. _element-name-example-1:

Example of general editorial notes:
-----------------------------------

.. code-block:: xml

  ...
  <front>
    <journal-meta> ... </journal-meta>
    <article-meta> ...  </article-meta>
    ...
    <notes>
      <sec>
        <title>...</title>
        <p>...</p>
      </sec>
    </notes>
  </front>
  ...


.. _element-name-example-2:

Example of general editorial notes without a title:
---------------------------------------------------

.. code-block:: xml

  ...
  <front>
    <journal-meta> ... </journal-meta>
    <article-meta> ...  </article-meta>
    ...
    <notes>
      <sec>
        <p>General editorial note...</p>
      </sec>
    </notes>
  </front>
  ...


.. _element-name-example-3:

Example of editorial notes for issue and article:
-------------------------------------------------

.. code-block:: xml

  ...
  <front>
    <journal-meta> ... </journal-meta>
    <article-meta> ...  </article-meta>
    <notes>
      <sec sec-type="issue-note">
        <title>Issue Editorial Note</title>
        <p>Issue editorial note....</p>
      </sec>
      <sec sec-type="article-note">
        <title>Article Editorial Note</title>
        <p>Article editorial note...</p>
      </sec>
    </notes>  
  </front>
  ...

.. {"reviewed_on": "20190422", "by": "fabio.batalha@erudit.org"}