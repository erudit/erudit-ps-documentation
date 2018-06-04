.. _element-verse-group:

<verse-group>
=============

+----------------------------------------+--------------------+
| Appears in                             | Frequency          |
+========================================+====================+
| :ref:`element-app`                     | Zero or more times |
+----------------------------------------+--------------------+
| ``<app-group>``                        | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-body`                    | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-boxed-text`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-disp-quote`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-p`                       | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-ref-list`                | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-sec`                     | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-supplementary-material`  | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-verse-group`             | Zero or more times |
+----------------------------------------+--------------------+

This element is used to display poems, verses or music. The element :ref:`element-attrib` can also be inserted to identify the author, and :ref:`element-label` to identify the title of the poem, verse, etc.

Example:

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
