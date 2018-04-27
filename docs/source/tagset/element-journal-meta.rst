.. _element-journal-meta:

<journal-meta>
==============

+------------------------+------------+
| Appears in             | frequency  |
+========================+============+
| :ref:`element-article` | Once       |
+------------------------+------------+


The metadata of the journal is identified at the element ``<journal-meta>``.

.. note:: 
 * Check the `ISSN <https://portal.issn.org/>`_ portal for journals metadata.

Elements found in ``<journal-meta>``:

+----------------------------------------+
| Tags                                   |
+========================================+
| :ref:`element-journal-id`              |
+----------------------------------------+
| :ref:`element-journal-title-group`     |
+----------------------------------------+
| :ref:`element-issn`                    |
+----------------------------------------+
| :ref:`element-publisher`               |
+----------------------------------------+

Example:

.. code-block:: xml

   ...
   <journal-meta>
        <journal-id journal-id-type="publisher-id">rum</journal-id>
        <journal-id journal-id-type="doi">rum</journal-id>
        <journal-title-group>
             <journal-title>Revue de l'Université de Moncton</journal-title>
        </journal-title-group>
        <issn pub-type="epub">1712-2139</issn>
        <issn pub-type="ppub">0316-6368</issn>
        <publisher>
             <publisher-name>Revue de l'Université de Moncton</publisher-name>
        </publisher>
   </journal-meta>
   ...

.. {"reviewed_on": "201804626", "by": "fabio.batalha@erudit.org"}
