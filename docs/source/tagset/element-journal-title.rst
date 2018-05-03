.. _element-journal-title:

<journal-title>
===============

Mandatory attributes:

  * ``@xml:lang``

+-------------------------------------+------------+
| Appears in                          | Frequency  |
+=====================================+============+
| :ref:`element-journal-title-group`  | Once       |
+-------------------------------------+------------+

Contains the long form of the title according to its :term:`ISSN` record.

Example:

.. code-block:: xml

  ...
  <journal-meta>
    ...
    <journal-title-group>
      <journal-title xml:lang="fr">Revue de l'Université de Moncton</journal-title>
      ...
    </journal-title-group>
    ...
  </journal-meta>
  ...


.. {"reviewed_on": "20180427", "by": "fabio.batalha@erudit.org"}
