.. _element-label:

<label>
=======

+----------------------------------------+--------------------+
| Appears in                             | Frequency          |
+========================================+====================+
| :ref:`element-aff`                     | Zero or more times |
+-------------------------------------------+-----------------+
| :ref:`element-app`                     | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-boxed-text`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-corresp`                 | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-def-list`                | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-disp-formula`            | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-fig`                     | Once               |
+----------------------------------------+--------------------+
| :ref:`element-fn`                      | Zero or more times |
+----------------------------------------+--------------------+
| ``glossary``                           | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-list`                    | Zero or more times |
+----------------------------------------+--------------------+
| ``list-item``                          | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-media`                   | Once               |
+----------------------------------------+--------------------+
| :ref:`element-ref`                     | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-sec`                     | Once               |
+----------------------------------------+--------------------+
| :ref:`element-supplementary-material`  | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-table-wrap`              | Once               |
+----------------------------------------+--------------------+
| :ref:`element-verse-group`             | Zero or more times |
+----------------------------------------+--------------------+

``<label>`` is meant to identify, numerically and/or alphabetically, a group of elements of a specific type.

Examples:

 * :ref:`element-label-example-1`
 * :ref:`element-label-example-2`
 * :ref:`element-label-example-3`
 * :ref:`element-label-example-4`

.. _element-label-example-1:

Example in ``<aff>``:
---------------------


.. code-block:: xml

    <aff id="aff01">
        <label>a</label>
        ...
    </aff>

.. _element-label-example-2:

Example em ``<fig>``:
---------------------

.. code-block:: xml

    <fig id="f01">
        <label>Figure 1</label>
        ...
    </fig>


.. _element-label-example-3:

Example in ``<table-wrap>``:
----------------------------

.. code-block:: xml

    <table-wrap id="t01">
        <label>Table 1</label>
        ...
    </table-wrap>


.. _element-label-example-4:

Example in ``<ref>``:
---------------------

.. code-block:: xml

    <ref id="B01">1</ref>
        <label>1</label>
        ...
    </ref>