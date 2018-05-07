.. _element-elocation-id:

<elocation-id>
==============

+----------------------------------+------------------+
| Appears in                       | Frequency        |
+==================================+==================+
| :ref:`element-article-meta`      | Zero or one time |
+----------------------------------+------------------+
| :ref:`element-element-citation`  | Zero or one time |
+----------------------------------+------------------+

Electronic identifier that replaces the sequential pagination of a document. 

.. note::

    This element should not be used combined with the elements :ref:`fpage` and/or :ref:`lpage`.

Example in :ref:`element-article-meta`:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <volume>10</volume>
        <issue>2</issue>
        <elocation-id>0102961</elocation-id>
        ...
    </article-meta>
    ...


Example in :ref:`elemento-element-citation`:

.. code-block:: xml

    ...
    <element-citation publication-type="journal">
        ...
        <source>PLoS ONE</source>
        <volume>6</volume>
        <elocation-id>e27721</elocation-id>
    </element-citation>
    ...


.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}
