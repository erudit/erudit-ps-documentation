.. _element-attrib:

<attrib>
========

+----------------------------------------+--------------------+
| Appears in                             | Frequency          |
+========================================+====================+
| :ref:`element-boxed-text`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-disp-quote`              | Zero or more times |
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

.. note::

  In :term:`JATS`, a variety of elements could be used inside ``<attrib>``. In the scope of the :term:`Érudit PS`, only the elements :ref:`element-email`, :ref:`element-title`, :ref:`element-uri` and a plain text ``text()`` will be recognized.

Example in figure:

.. code-block:: xml

  ...
  <fig id="f02" fig-type="other">
    <label>Figure 2</label>
      <caption>
        <title>Produtividade das variantes lexicais para a questão 132 do QSL segundo a região administrativa</title>
      </caption>
      <graphic xlink:href="figure.tiff"/>
      <attrib>Fonte: Banco de dados do ALiB (2013).</attrib>
  </fig>
  ...

.. note:: 

  For figures, the element :ref:`element-attrib` should be inserted bellow the element :ref:`element-graphic`.


Example in verses:

.. code-block:: xml

  <verse-group>
    <label>A verse sample</label>
    <verse-line>Sampling a verse</verse-line>
    <verse-line>Sampling what?</verse-line>
    <verse-line>A simple verse</verse-line>
    <verse-line>A unmeaning verse.</verse-line>
    <attrib>Anonymous</attrib>
  </verse-group>

.. {"reviewed_on": "20180603", "by": "fabio.batalha@erudit.org"}
