.. _element-trans-title-group:

<trans-title-group>
===================

Mandatory Attributes:

  1. ``@xml:lang``

+-----------------------------+--------------------+
| Appears at                  | Frequency          |
+=============================+====================+
| :ref:`element-title-group`  | Zero or more times |
+-----------------------------+--------------------+


Used to show the translated article title or a group of translations for the article title. The
attribute ``@xml:lang`` is mandatory and identifies the language of the translated title.


Example:

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
