.. _element-abbrev-journal-title:

<abbrev-journal-title>
======================

Mandatory attributes:

  1. ``@abbrev-type="erudit"``

+-------------------------------------+-------------------------+
| Appears in                          | Frequency               |
+=====================================+=========================+
| :ref:`element-journal-title-group`  | Once or more times      |
+-------------------------------------+-------------------------+


Specifies the abbreviated form of the journal title.

Érudit requires that at least one element ``abbrev-journal-title`` containing the attribute ``@abbrev-type`` with the value **erudit** should be present at the XML. It's content should be the abbreviated journal title as it suggested by Érudit.

.. note::

    The Érudit Journal ID should be defined at the :ref:`element-journal-id`, not in the ``abbrev-journal-title``. 

Example:

.. code-block:: xml

    ...
    <journal-title-group>
        <abbrev-journal-title abbrev-type="erudit">Rev Univ de Moncton</abbrev-journal-title>
    </journal-title-group>
    ...

.. {"reviewed_on": "20180430", "by": "fabio.batalha@erudit.org"}
