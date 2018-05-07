.. _element-season:

<season>
========

+----------------------------------+-----------------+
| Appears in                       | Frequency       |
+==================================+=================+
| :ref:`element-element-citation` | Zero or one time |
+----------------------------------+-----------------+
| :ref:`element-product`          | Zero or one time |
+----------------------------------+-----------------+
| :ref:`element-pub-date`         | Zero or one time |
+----------------------------------+-----------------+

This element can occur in :ref:`pub-date` to identify a month range (see Note below), and in :ref:`element-citation` and :ref:`product` to identify the season in a bibliographic reference.

Examples:

    * :ref:`element-season-example-1`
    * :ref:`element-season-example-2`


.. _element-season-example-1:

Example of ``<season>`` as a season:
------------------------------------

.. code-block:: xml

    ...
    <back>
        ...
        <ref-list>
            <ref>
                ...
                <season>Autumn</season>
                ...
            </ref>
        </ref-list>
        ...
    </back>


.. _element-season-example-2:

Example ``<season>`` as a month range:
--------------------------------------

.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <pub-date pub-type="epub">
                <season>Nov-Dec</season>
                <year>2013</year>
            </pub-date>
            ...
        </article-meta>
        ...
    </front>
    ...


.. note:: 

  Always use the following three letter English abbreviations for months, separated by a hyphen in the case of a month range: Jan, Feb, Mar, Apr, May, Jun, Jul, Aug, Sep, Oct, Nov, Dec.

.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}