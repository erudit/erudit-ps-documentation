.. _element-trans-title-group:

<trans-title-group>
===================

Mandatory Attributes:

  1. ``@xml:lang``

+-------------------------------------+--------------------+
| Appears at                          | Frequency          |
+=====================================+====================+
| :ref:`element-journal-title-group`  | Zero or more times |
+-------------------------------------+--------------------+
| :ref:`element-title-group`          | Zero or more times |
+-------------------------------------+--------------------+


Used to show the translated **article title** or **journal title** or a group of translations for the **article title** and **journal title**. The
attribute ``@xml:lang`` is mandatory and identifies the language of the translated title.


Examples:

  * :ref:`element-trans-title-example-1`
  * :ref:`element-trans-title-example-2`


.. _element-trans-title-example-1:

Example of ``trans-title-group`` in ``journal-title-group``
-----------------------------------------------------------

.. code-block:: xml

    ...
    <journal-title-group>
        <journal-title>Revue de l'Université de Moncton</journal-title>
        <trans-title-group xml:lang="pt">
            <trans-title>Revista da Universidade de Moncton</trans-title>
        </trans-title-group>
    </journal-title-group>
    ...

.. _element-trans-title-example-2:

Example of ``trans-title-group`` in ``title-group``
---------------------------------------------------

.. code-block:: xml

    ...
    <title-group>
        <article-title>De la préservation linguistique et nationale: la qualité de la langue de la jeunesse acadienne, un débat linguistique idéologique</article-title>
        <trans-title-group xml:lang="pt">
            <trans-title>Preservaçao linguistica e nacional: a qualidade da linguagem da juventude acadiana, um debate linguistico ideológico</trans-title>
        </trans-title-group>
    </title-group>
    ...

.. {"reviewed_on": "201804627", "by": "fabio.batalha@erudit.org"}
