.. _element-table-wrap:

<table-wrap>
============

Mandatory attributes:

  1. ``@id`` (ver :ref:`id-attribution-tips`)

+----------------------------------------+--------------------+
| Appears in                             | Frequency          |
+========================================+====================+
| :ref:`element-app`                     | Zero or more times |
+----------------------------------------+--------------------+
| ``<app-group>``                        | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-body`                    | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-glossary`                | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-p`                       | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-sec`                     | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-supplementary-material`  | Zero or more times |
+----------------------------------------+--------------------+

Specifies all the parts of a single table, including :ref:`element-label`, :ref:`element-caption` and, if it exists, :ref:`element-table-wrap-foot`.

.. note::

  The element :ref:`label` is mandatory in Érudit Article.

Example:

.. code-block:: xml

    ...
    <table-wrap id="t5">
      <label>Table 5</label>
      <caption>
        <title>The values for suppliers</title>
      </caption>
      <table>
        <thead>
          <tr>
            <th rowspan="3">Proposed rage for 2018</th>
          </tr>
          <tr>
            <th>Incoming in 12 months</th>
            <th>Annexe I - Comercial</th>
            <th>Annexe II - Industry</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>from $225,000.01 to $450,000.00</td>
            <td>4.00%</td>
            <td>4.50%</td>
          </tr>
          <tr>
            <td>from $450,000.01 to $900,000.00</td>
            <td>8.25%</td>
            <td>8.00%</td>
          </tr>
          <tr>
            <td>from $900.000,01 to $1.800.000,00</td>
            <td>11.25%</td>
            <td>12.25%</td>
          </tr>
        </tbody>
      </table>
      <table-wrap-foot>
        <fn id="TFN1">
           <p>the annexe 2 information is meaningfull</p>
        </fn>
      </table-wrap-foot>
    </table-wrap>
    ...


.. {"reviewed_on": "20180601", "by": "fabio.batalha@erudit.org"}
