.. _element-abbrev-journal-title:

<abbrev-journal-title>
======================

Mandatory attributes:

  1. ``@abbrev-type="publisher"``

+-------------------------------------+------------+
| Appears in                          | Frequency  |
+=====================================+============+
| :ref:`element-journal-title-group`  | Once       |
+-------------------------------------+------------+


Specifies the abbreviated form of the journal title according to its :term:`ISSN` record.

.. note:: 
 * Check the `ISSN <https://portal.issn.org/>`_ website.

Example:

.. code-block:: xml

    ...
    <journal-title-group>
        <abbrev-journal-title abbrev-type="publisher">>Rev Univ de Moncton</abbrev-journal-title>
    </journal-title-group>
    ...

.. {"reviewed_on": "20180427", "by": "fabio.batalha@erudit.org"}
