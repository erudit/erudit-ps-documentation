.. _element-trans-title:

<trans-title>
=============

+-----------------------------------+------------+
| Appears at                        | Frequency  |
+===================================+============+
| :ref:`element-trans-title-group`  | Once       |
+-----------------------------------+------------+


Identifies the translated title of the article or journal. The attribute ``@xml:lang`` should be explicity defined in the parent element :ref:`element-trans-title-group`, not in ``trans-title``.


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
        <trans-title-group xml:lang="en">
            <trans-title>Preservación linguistica y nacional: la calidad de la lenguade la juventude acadiana, un debate linguistico ideologico</trans-title>
        </trans-title-group>
    </title-group>
    ...


.. {"reviewed_on": "201804627", "by": "fabio.batalha@erudit.org"}
