.. _element-page-range:

<page-range>
============

+----------------------------------+------------------+
| Appears in                       | Frequency        |
+==================================+==================+
| :ref:`element-element-citation`  | Zero or one time |
+----------------------------------+------------------+
| :ref:`element-product`           | Zero or one time |
+----------------------------------+------------------+

Identifies one or more page ranges found between the values of :ref:`element-fpage` and :ref:`element-lpage` in a bibliographic reference. Each page range can be composed of a numerical value (denoting a single page) or two numerical values separated by a hyphen (indicating a page range). Different page ranges are separated by a comma.

Example:

.. code-block:: xml

    ...
    <ref>
        <element-citation publication-type="book">
            ...
            <fpage>300</fpage>
            <lpage>420</lpage>
            <page-range>300-301, 305, 407-420</page-range>
            ...
        </element-citation>
        ...
    </ref>
    ...

.. note::

    A page range should be inserted after the information about the :ref:`last page`.


.. {"reviewed_on": "20180508", "by": "fabio.batalha@erudit.org"}
