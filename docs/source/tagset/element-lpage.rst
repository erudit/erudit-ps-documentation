.. _element-lpage:

<lpage>
=======

+----------------------------------+------------------+
| Appears in                       | Frequency        |
+==================================+==================+
| :ref:`element-article-meta`      | Zero or one time |
+----------------------------------+------------------+
| :ref:`element-element-citation`  | Zero or one time |
+----------------------------------+------------------+

Indicates the last page of the article.

.. note::

    This element should not be used combined with the element :ref:`elocation-id`.

Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <fpage>396</fpage>
        <lpage>452</lpage>
        ...
    </article-meta>
    ...

.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}
