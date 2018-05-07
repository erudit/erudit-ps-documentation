.. _element-fpage:

<fpage>
=======

+----------------------------------+------------------+
| Appears in                       | Frequency        |
+==================================+==================+
| :ref:`element-article-meta`      | Zero or one time |
+----------------------------------+------------------+
| :ref:`element-element-citation`  | Zero or one time |
+----------------------------------+------------------+


Indicates the first page of the article.

.. note::

    This element should not be used combined with the element :ref:`elocation-id`.


Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <fpage>17</fpage>
        <lpage>21</lpage>
        ...
    </article-meta>
    ...


This element may also be used with attribute ``@seq`` for issues where there is more than one article beginning on the same page. An alphanumeric sequence should differentiate an article from others on the same page. For example, if the first article begins on page 82, it should be given the sequence number “82a”; the letter “a” would be followed in sequence by “b” for a second article starting on the same page, and so on.

Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <fpage seq="a">82</fpage>
        <lpage>83</lpage>
        ...
    </article-meta>
    ...


.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}
