.. _element-attrib:

<attrib>
========

+----------------------------------------+--------------------+
| Appears in                             | Frequency          |
+========================================+====================+
| :ref:`element-boxed-text`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-fig`                     | Zero or more times |
+----------------------------------------+--------------------+
| ``<graphic>``                          | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-media`                   | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-supplementary-material`  | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-table-wrap`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-verse-group`             | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-table-wrap-foot`         | Zero or more times |
+----------------------------------------+--------------------+

Used to credit the author or licensor of the assets or content which require such attribution.

Example in figure:

.. code-block:: xml

  ...
  <fig id="f02" fig-type="other">
    <label>Figure 2</label>
      <caption>
        <title>Produtividade das variantes lexicais para a questão 132 do QSL segundo a região administrativa</title>
      </caption>
      <graphic xlink:href="0103-507X-rbti-26-02-0130-g02.tif"/>
      <attrib>Fonte: Banco de dados do ALiB (2013).</attrib>
  </fig>
  ...

.. note:: 

  For figures, the element :ref:`element-attrib` should be inserted bellow the element :ref:`element-graphic`.


Example in verses:

.. code-block:: xml

  ...
  <verse-group>
    <label>Porque é que um sono agita</label>
    <verse-line>E, num fiel regresso</verse-line>
    <verse-line>Ao que já era bruma,</verse-line>
    <verse-line>Sonolento me apresso</verse-line>
    <verse-line>Para coisa nenhuma.</verse-line>
    <attrib>Fernando Pessoa</attrib>
  </verse-group>
  ...

.. {"reviewed_on": "20180603", "by": "fabio.batalha@erudit.org"}
