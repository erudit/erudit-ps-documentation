.. _element-title-group:

<title-group>
=============

+------------------------------+------------+
| Appears in                   | Frequency  |
+==============================+============+
| :ref:`element-article-meta`  | Once       |
+------------------------------+------------+

Specifies the title or group of titles of the article. Elements :ref:`element-article-title` and :ref:`element-trans-title-group` are identified within it.


.. note::

    ``<title-group>`` should be inserted above the element :ref:`element-article-categories` or before :ref:`element-contrib-group`.

Examples:

* :ref:`element-titlegroup-example-1`
* :ref:`element-titlegroup-example-2`


.. _element-titlegroup-example-1:

Example of title in only one language:
--------------------------------------

.. code-block:: xml

    ...
    <article-meta>
      ...
      <title-group xml:lang="fr">
          <article-title>De la préservation linguistique et nationale: la qualité de la langue de la jeunesse acadienne, un débat linguistique idéologique</article-title>
      </title-group>
      ...
    </article-meta>
    ...


.. _element-titlegroup-example-2:

Example of title in the main language and translated titles:
------------------------------------------------------------

.. code-block:: xml

    ...
    <title-group>
        <article-title xml:lang="es">Conocimientos de los pediatras sobre la laringomalacia: ¿siempre es un proceso banal?</article-title>
        <trans-title-group xml:lang="en">
            <trans-title>Pediatrician knowledge about laryngomalacia: is it always a banal process?</trans-title>
        </trans-title-group>
    </title-group>
    ...
    


.. {"reviewed_on": "20180508", "by": "fabio.batalha@erudit.org"}