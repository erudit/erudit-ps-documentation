.. _element-counts:

<counts>
========

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-article-meta`  | Zero or more times |
+------------------------------+--------------------+

Element used to provide the precise count of the number of tables, figures, references, equations and pages present in the document. It should be inserted as the last item of :ref:`element-article-meta`.

The elements which identify the totals in the :term:`documento` are:

* ``<fig-count>``: Total number of figures
* ``<table-count>``: Total number of tables
* ``<equation-count>``: Total number of equations
* ``<ref-count>``: Total number of references
* ``<page-count>``: Total number of pages

.. note:: 

 * The order of the elements is important 
 * If the :term:`document` does not have any of the countable elements, this element should not be available in ``<counts>``. 

Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <counts>
            <fig-count count="5"/>
            <table-count count="3"/>
            <equation-count count="10"/>
            <ref-count count="26"/>
            <page-count count="6"/>
        </counts>
    </article-meta>
    ...

.. {"reviewed_on": "20180524", "by": "fabio.batalha@erudit.org"}
