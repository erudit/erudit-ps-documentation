.. _element-article-id:

<article-id>
============

Mandatory attributes:

  1. ``@pub-id-type``

+-------------------------------+--------------------+
| Appears in                    | Frenquency         |
+===============================+====================+
| :ref:`element-article-meta`   | Zero or more times |
+-------------------------------+--------------------+


Unique identifier of the document in a database.

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
        <article-id pub-id-type="publisher-id">1031001ar</article-id>
        <article-id pub-id-type="doi">10.7202/1031001ar</article-id>
        ...
    </article-meta>
    ...

.. note::

    :term:`Érudit PS` expects to receive the DOI numbers in its raw form. It means will not be accepted any content like http://dx.doi.org/10.7202/1031001ar, but only  10.7202/1031001ar



