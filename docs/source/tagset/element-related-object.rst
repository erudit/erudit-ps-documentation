.. _element-related-object:

<related-object>
================

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

Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <related-object content-type="review" document-type="book">Book Title</related-object>
        ...
    </article-meta>
    ...

.. code-block:: xml

    ...
    <article-meta>
        ...
        <related-object content-type="review" document-type="book-chapter">Chapter Title</related-object>
        ...
    </article-meta>
    ...

.. code-block:: xml

    ...
    <article-meta>
        ...
        <related-object content-type="review" document-type="article">Article Title</related-object>
        ...
    </article-meta>
    ...

.. {"reviewed_on": "20190226", "by": "fabio.batalha@erudit.org"}
