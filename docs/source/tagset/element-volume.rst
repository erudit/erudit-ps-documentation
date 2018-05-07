.. _element-volume:

<volume>
========

+----------------------------------+--------------------+
| Appears in                       | Frequency          |
+==================================+====================+
| :ref:`element-article-meta`      | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-element-citation`  | Zero or more times |
+----------------------------------+--------------------+
| :ref:`elemeno-product`           | Zero or more times |
+----------------------------------+--------------------+


Represents the volume of a publication.

.. note:

  Do not use this element to identify a supplement. See :ref:`element-issue` for supplement numbers.

Examples:

 * :ref:`element-volume-example-1`
 * :ref:`element-volume-example-2`


.. _element-volume-example-1:


Example of  ``<volume>`` in :ref:`article-meta`:
------------------------------------------------

 * Refers to a issue: volume 32, number 12 (``v32n12``):


.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <volume>32</volume>
            <issue>12</issue>
            ...
        </article-meta>
        ...
    </front>
    ...


.. _element-volume-example-2:

Example of ``<volume>`` in :ref:`<element-citation>`:
-----------------------------------------------------

 * Refers to a volume in a reference


.. code-block:: xml

    ...
    <ref id="B01">
        ...
        <source>Journal Title</source>
        <volume>32</volume>
        <issue>12</issue>
        ...
    </ref>
    ...

.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}
