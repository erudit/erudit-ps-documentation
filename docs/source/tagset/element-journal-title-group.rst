.. _element-journal-title-group:

<journal-title-group>
=====================

+------------------------------+------------+
| Appears in                   | frequency  |
+==============================+============+
| :ref:`element-journal-meta`  | Once       |
+------------------------------+------------+

Contains the elements which identify the metadata related to the title of the journal.

Usual elements found in ``<journal-title-group>``:

+------------------------------------------+
| Tags                                     |
+==========================================+
| :ref:`element-journal-title`             |
+------------------------------------------+
| :ref:`element-journal-abbreviated-title` |
+------------------------------------------+

Example:

.. code-block:: xml

    ...
    <journal-meta>
        ...
        <journal-title-group>
            <journal-title>Revue de l'Université de Moncton</journal-title>
            <journal-abbreviated-title>Rev Univ Mon</journal-abbreviated-title>
            ...
        </journal-title-group>
        ...
    </journal-meta>
    ...


.. {"reviewed_on": "20180426", "by": "fabio.batalha@erudit.org"}
