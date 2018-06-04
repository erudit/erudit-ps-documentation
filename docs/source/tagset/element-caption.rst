.. _element-caption:

<caption>
=========

+----------------------------------------+--------------------+
| Appears in                             | Frequency          |
+========================================+====================+
| :ref:`element-boxed-text`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-disp-formula`            | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-fig`                     | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-media`                   | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-supplementary-material`  | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-table-wrap`              | Zero or more times |
+----------------------------------------+--------------------+

Describes a caption for various types of objects. ``<caption>`` involves the element ``<title>`` to hold the descriptive text of a table, figure, media, formula or similar object, as well as the element ``<p>`` to identify additional text.

Examples:

  * :ref:`element-caption-example-1`
  * :ref:`element-caption-example-2`


.. _element-caption-example-1:

Example of ``<fig>`` with ``<caption>``:
----------------------------------------

.. code-block:: xml

    ...
    <fig id="f03">
        <label>Figura 3</label>
        <caption>
            <title>Percentual de atividade mitocondrial (método MTT) das células dos diferentes grupos experimentais em relação às células do grupo controle</title>
        </caption>
        <graphic xlink:href="figure.tiff"/>
    </fig>
    ...


.. _element-caption-example-2:

Example of ``<fig>`` with ``<caption>`` with aditional information:
-------------------------------------------------------------------

.. code-block:: xml

  ...
  <fig id="f03">
        <label>Figura 4</label>
        <caption>
            <title>Despesas realizadas pelas IES brasileiras em 2005 como percentuais do PIB</title>
            <p>(Valores em R$ bilhões, a preços de janeiro de 2010, corrigidos pelo IPCA)</p>
        </caption>
        <graphic xlink:href="figure.tiff"/>
    </fig>
    ...

.. {"reviewed_on": "20180603", "by": "fabio.batalha@erudit.org"}
