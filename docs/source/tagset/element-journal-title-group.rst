.. _element-journal-title-group:

<journal-title-group>
=====================

+------------------------------+------------+
| Appears in                   | frequency  |
+==============================+============+
| :ref:`element-journal-meta`  | Once       |
+------------------------------+------------+

Contains the elements which identify the metadata related to the title of the journal.

Elements found in ``<journal-title-group>``:

+------------------------------------------+
| Tags                                     |
+==========================================+
| :ref:`element-journal-title`             |
+------------------------------------------+
| :ref:`element-journal-subtitle`          |
+------------------------------------------+
| :ref:`element-trans-title`               |
+------------------------------------------+
| :ref:`element-abbrev-journal-title`      |
+------------------------------------------+

Example:

.. code-block:: xml

    ...
    <journal-meta>
        ...
        <journal-title-group>
            <journal-title>Revue de l'Université de Moncton</journal-title>
            <abbrev-journal-title abbrev-type="erudit">Rev Univ Mon</abbrev-journal-title>
            ...
        </journal-title-group>
        ...
    </journal-meta>
    ...


.. {"reviewed_on": "20180426", "by": "fabio.batalha@erudit.org"}
