.. _element-related-object:

<related-object>
================

Mandatory attributes:

  1. ``@content-type``
  2. ``@document-type``

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+

This is an optional element used to make reference to a resource in which the
article was based. It is usually used in review articles to make reference to the
reviewed souce, ex: book, article, thesis, etc.

.. note::

    Even the **related-object** element is allowed inside other elements according to JATS
    specifications. For Érudit Publishing Schema, this element will be recoginized only
    if available in the element **article-meta** only for the purpose discribed above.

The recoginized values for the attribute **@document-type** are:

    * book
    * book-chapter
    * article

The recoginized values for the attribute **@content-type** are:

    * reviewed-document

Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <surtitre>Les comptes rendus</surtitre>
        <title-group>
          <sub-title xml:lang="fr">Les comptes rendus</sub-title>
        </title-group>
        <related-object content-type="reviewed-document" document-type="article"><italic>Emploi. Économie Sociale. Développement local. Les nouvelles filières</italic>, Yvan Comeau, Louis Favreau, Benoît Lévesque et Marguerite Mendell, Sainte-Foy, Presses de l’Université du Québec, 2001, 336 p.</related-object>
        ...
    </article-meta>
    ...


.. code-block:: xml

    ...
    <article-meta>
        ...
        <related-object content-type="reviewed-document" document-type="book">Book Title</related-object>
        ...
    </article-meta>
    ...

.. code-block:: xml

    ...
    <article-meta>
        ...
        <related-object content-type="reviewed-document" document-type="book-chapter">Chapter Title</related-object>
        ...
    </article-meta>
    ...

.. code-block:: xml

    ...
    <article-meta>
        ...
        <related-object content-type="reviewed-document" document-type="article">Article Title</related-object>
        ...
    </article-meta>
    ...

.. {"reviewed_on": "20190226", "by": "fabio.batalha@erudit.org"}
