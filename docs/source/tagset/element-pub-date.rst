.. _element-pub-date:

<pub-date>
==========

Mandatory attributes:

  1. ``@date-type``
  2. ``@publication-format``

+------------------------------+------------+
| Appears in                   | Frequency  |
+==============================+============+
| :ref:`element-article-meta`  | Two times  |
+------------------------------+------------+


The publication date of an article and it's issue uses the element ``<pub-date>`` which may contain the elements :ref:`day`, :ref:`month`, :ref:`season` and must contain :term:`year`. ``<pub-date>`` must be accompanied by the attribute ``@publication-format`` and ``@date-type`` where:

``@publication-format`` can be **ppub** if there is a publication date for a print version of the article, and **epub** to identify the electronic publication date.

``@date-type`` can be **collection** or **pub** where:

    * **pub** represents the article publication date
    * **collection** represents the publication date defined by the journal periodicity

.. note::

    It is not necessary to have the attribute ``@publication-format`` when the attribute ``@pub-type`` has the value **collection**. See the examples bellow.

For Érudit PS will be mandatory to have at least one ``<pub-date>`` element inside :ref:`<article-meta>` with the publication date defined by the journal periodicity and expressed by the attribute ``@date-type=collection``. The article and journal publishing dates may differs for many reasons. 

.. note::

    The use of the attribute ``@pub-type`` is deprecated in JATS 1.1, and consequently it is not accepted in :term:`Érudit PS`.

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
        <pub-date publication-format="epub" date-type="pub">
            <season>Jan-Feb</season>
            <year>2014</year>
        </pub-date>
        <pub-date publication-format="ppub" date-type="pub">
            <season>Jan-Feb</season>
            <year>2014</year>
        </pub-date>
        <pub-date date-type="collection">
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
        <pub-date publication-format="epub" date-type="pub">
            <day>10</day>
            <month>01</month>
            <year>2014</year>
        </pub-date>
        <pub-date publication-format="ppub" date-type="pub">
            <day>21</day>
            <month>02</month>
            <year>2014</year>
        </pub-date>
        <pub-date date-type="collection">
            <season>Jan-Feb</season>
            <year>2014</year>
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
        <pub-date publication-format="epub" date-type="pub">
            <day>17</day>
            <month>03</month>
            <year>2014</year>
        </pub-date>
        <pub-date date-type="collection">
            <year>2015</year>
        </pub-date>
        ...
    </article-meta>
    ...

