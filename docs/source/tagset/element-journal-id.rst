.. _element-journal-id:

<journal-id>
============

Mandatory Attributes:

  1. ``@journal-id-type``

+------------------------------+-------------------+
| Contained at                 | Frequency         |
+==============================+===================+
| :ref:`element-journal-meta`  | One or more time  |
+------------------------------+-------------------+

Have the unique id of the journal indexed and published by a publishing house.

It is mandatory to have at least one element journal ``<journal-id>`` with the value ``publisher-id`` in the attribute ``@journal-id-type``. In this occurency the id should be the journal identifier at Érudit.

The allowed values for ``@journal-id-type`` are:

+---------------+-----------------------------------------+
| Value         | Description                             |
+===============+=========================================+
| publisher-id  | Journal id at Érudit database           |
+---------------+-----------------------------------------+

Example:

.. code-block:: xml

    ...
    <journal-meta>
        ...
        <journal-id journal-id-type="publisher-id">mioc</journal-id>
        <journal-id journal-id-type="nlm-ta">Mem Inst Oswaldo Cruz</journal-id>
        ...
    </journal-meta>
    ...


.. {"reviewed_on": "20180422", "by": "fabio.batalha@erudit.org"}