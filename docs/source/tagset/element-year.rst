.. _element-year:

<year>
======

+----------------------------------+---------------------+
| Appears in                       | Frequency           |
+==================================+=====================+
| :ref:`element-date`              | Once                |
+----------------------------------+---------------------+
| :ref:`element-element-citation`  | Zero or more times  |
+----------------------------------+---------------------+
| :ref:`element-product`           | Zero ou more times  |
+----------------------------------+---------------------+
| :ref:`element-pub-date`          | Once                |
+----------------------------------+---------------------+

Identifies the year in references. It can be the year of publication of a document, the production year of a software, the creation year of a database, etc. It can also be used in :ref:`front` to identify the publication year of an article see :term:`pub-date` or :term:`product`.

Examples:

  * :ref:`element-year-example-1`
  * :ref:`element-year-example-2`
  * :ref:`element-year-example-3`


.. _element-year-example-1:

Example of ``<year>`` in ``<article-meta>``:
--------------------------------------------

.. code-block:: xml

    ...
    <article-meta>
    ...
        <pub-date pub-type="epub-ppub">
            <season>Apr-Jun</season>
            <year>2016</year>
        </pub-date>
    ...
    </article-meta>
 ...


.. _element-year-example-2:

Example of ``<year>`` in ``<element-citation>``:
------------------------------------------------

.. code-block:: xml

    ...
    <element-citation publication-type="journal">
        ...
        <source>Pediatric aerodigestive disorders</source>
        <year>2009</year>
        ...
    </element-citation>
    ...


.. _element-year-example-3:

Example of ``<year>`` in ``<product>``:
---------------------------------------

.. code-block:: xml

    ...
    <product product-type="book">
        ...
        <year>2014</year>
        <source>A revision of Axinaea (Melastomataceae)</source>
        ...
   </product>
   ...

.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}