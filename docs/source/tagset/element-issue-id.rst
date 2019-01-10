.. _element-issue-id:

<issue-id>
============

Mandatory attributes:

  1. ``@pub-id-type``

+-------------------------------+--------------------+
| Appears in                    | Frenquency         |
+===============================+====================+
| :ref:`element-article-meta`   | Zero or more times |
+-------------------------------+--------------------+


Unique identifier of the issue the document belongs to.

The element must have the attribute ``@pub-id-type``, which is used to identify the type of the identifier.

The attribute ``@pub-id-type`` allows the use of some values, see `JATS for reference <https://jats.nlm.nih.gov/publishing/tag-library/1.2d1/attribute/pub-id-type.html>`_.

As best practice :term:`Érudit PS` requests the use of at least one of the following values:

+--------------------+-------------------------------------------------------+
| Value              | Description                                           |
+====================+=======================================================+
| doi                | *Digital Object Identifier*.                          |
+--------------------+-------------------------------------------------------+
| publisher-id       | Érudit Article ID.                                    |
+--------------------+-------------------------------------------------------+

Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <issue-id pub-id-type="publisher-id">approchesind0522</article-id>
        ...
    </article-meta>
    ...

.. {"reviewed_on": "20190110", "by": "fabio.batalha@erudit.org"}