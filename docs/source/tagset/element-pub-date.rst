.. _element-pub-date:

<pub-date>
==========

Mandatory attributes:

  1. ``@pub-type``

+------------------------------+------------+
| Appears in                   | Frequency  |
+==============================+============+
| :ref:`element-article-meta`  | Once       |
+------------------------------+------------+


The publication date of an article uses the element ``<pub-date>`` which may contain the elements :ref:`day`, :ref:`month`, :ref:`season` and must contain :term:`year`. ``<pub-date>`` must be accompanied by the attribute ``@pub-type`` which can be **epub** or **ppub** if there is a print version for the issue, or only epub when:

    * there is only an online version;
    * it is a Continuous Publication;
    * it is Ahead of Print

Examples:

    * :ref:`element-pubdate-example-1`
    * :ref:`element-pubdate-example-2`
    * :ref:`element-pubdate-example-3`

    

.. _element-pubdate-example-1: 

Example of ``<pub-date>`` of a document in a print and electronic version with ``<season>``:
--------------------------------------------------------------------------------------------

.. code-block:: xml

    ...
    <article-meta>
        ...
        <pub-date pub-type="epub-ppub">
            <season>Jan-Feb</season>
            <year>2014</year>
        </pub-date>
        ...
    </article-meta>
    ...

.. _element-pubdate-example-2: 

Example of ``<pub-date>`` of a document in a print and electronic version with ``<month>`` e ``<day>``:
-------------------------------------------------------------------------------------------------------

.. code-block:: xml

    ...
    <article-meta>
        ...
        <pub-date pub-type="epub-ppub">
            <day>21</day>
            <month>07</month>
            <year>2016</year>
        </pub-date>
        ...
    </article-meta>
    ...


.. _element-pubdate-example-3:

Example of ``<pub-date>`` of a document available only in electronic version:
-----------------------------------------------------------------------------

.. code-block:: xml

    ...
    <article-meta>
        ...
        <pub-date pub-type="epub">
            <day>17</day>
            <month>03</month>
            <year>2014</year>
        </pub-date>
        ...
    </article-meta>
    ...

