.. _element-sub:

<subtitle>
===============

+----------------------------------+------------------+
| Appears in                       | Frequency        |
+==================================+==================+
| :ref:`element-title-group`       | Zero or once     |
+----------------------------------+------------------+

Used in :ref:`element-title-group` to identify the sub-title of the article.

* In :ref:`element-title-group`, the attribute ``@xml:lang`` should be used. Even it is not mandatory, it is an :term:`Érudit PS` recomendation.

Example:

.. code-block:: xml

    ...
    <article-meta>
      ...
      <title-group>
          <article-title xml:lang="fr">De la préservation linguistique et nationale</article-title>
          <sub-title xml:lang="fr">la qualité de la langue de la jeunesse acadienne, un débat linguistique idéologique</sub-title>
      </title-group>
      ...
    </article-meta>
    ...

.. {"reviewed_on": "20180530", "by": "fabio.batalha@erudit.org"}