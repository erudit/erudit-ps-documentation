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

``@publication-format`` can be **epub-ppub** if there is a print version for the article, or only **epub** when:

    * there is only an online version;
    * it is a Continuous Publication;
    * it is Ahead of Print;

``@date-type`` can be all the `valid types <https://jats.nlm.nih.gov/publishing/tag-library/1.2d1/attribute/date-type.html>`_ specified in :term:`JATS` including the value **issue** recognized by the :term:`Érudit PS`.

.. note::

    The use of the attribute ``@pub-type`` is deprecated in JATS 1.1, and consequently it is not accepted in :term:`Érudit PS`.

For Érudit PS will be mandatory to have 2 ``<pub-date>`` elements inside :ref:`<article-meta>`. One to identify the article publication date, and another to specify the issue publication date, that may differs for many reasons.

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
        <pub-date publication-format="epub-ppub" date-type="pub">
            <season>Jan-Feb</season>
            <year>2014</year>
        </pub-date>
        <pub-date date-type="issue">
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
        <pub-date publication-format="epub-ppub" date-type="pub">
            <day>21</day>
            <month>02</month>
            <year>2018</year>
        </pub-date>
        <pub-date date-type="issue">
            <year>2017</year>
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
        ...
    </article-meta>
    ...

