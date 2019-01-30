.. _element-abbrev-journal-title:

<abbrev-journal-title>
======================

Mandatory attributes:

  1. ``@abbrev-type="publisher"``

+-------------------------------------+-------------------------+
| Appears in                          | Frequency               |
+=====================================+=========================+
| :ref:`element-journal-title-group`  | Once or more times      |
+-------------------------------------+-------------------------+


Specifies the abbreviated form of the journal title.

Érudit requires that at least one element ``abbrev-journal-title`` containing the attribute ``@abbrev-type`` with the value **publisher** should be present at the XML. It's content should be the abbreviated journal title as it is suggested by Érudit.

.. note::

    The Érudit Journal ID should be defined in the element :ref:`element-journal-id`, not in the ``abbrev-journal-title``. 

Example:

.. code-block:: xml

    ...
    <journal-meta>
        <journal-id journal-id-type="publisher-id">approchesind0522</journal-id>
        <journal-title-group>
            <journal-title>Approches inductives</journal-title>
            <journal-subtitle>Travail intellectuel et construction des connaissances</journal-subtitle>
            <abbrev-journal-title abbrev-type="publisher">approchesind</abbrev-journal-title>
            <abbrev-journal-title abbrev-type="nlm">Appr. Induc.</abbrev-journal-title>
        </journal-title-group>
        ...
    </journal-meta>
    ...

.. {"reviewed_on": "20190130", "by": "fabio.batalha@erudit.org"}
