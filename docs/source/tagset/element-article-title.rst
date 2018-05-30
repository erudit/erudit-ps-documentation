.. _element-article-title:

<article-title>
===============

+----------------------------------+------------------+
| Appears in                       | Frequency        |
+==================================+==================+
| :ref:`element-title-group`       | Once             |
+----------------------------------+------------------+
| :ref:`element-element-citation`  | zero or one time |
+----------------------------------+------------------+

Used in :ref:`element-title-group` to identify the title of the article, or to specify the title of a document appearing in the references in :ref:`element-element-citation`.

* In :ref:`element-title-group`, the attribute ``@xml:lang`` should be used. Even it is not mandatory, it is an :term:`Érudit PS` recomendation.
* In :ref:`element-element-citation` the attribute ``@xml:lang`` should not be used.

Examples:

  * :ref:`element-article-title-example-1`
  * :ref:`element-article-title-example-2`

.. _element-article-title-example-1:

Example of ``<article-title>`` in :ref:`element-article-meta`:
--------------------------------------------------------------

.. code-block:: xml

    ...
    <article-meta>
      ...
      <title-group>
          <article-title xml:lang="en">De la préservation linguistique et nationale</article-title>
          <sub-title>la qualité de la langue de la jeunesse acadienne, un débat linguistique idéologique</sub-title>
      </title-group>
      ...
    </article-meta>
    ...

.. _element-article-title-example-2:

Example of ``<article-title>`` in :ref:`element-element-citation`:
------------------------------------------------------------------

.. code-block:: xml

    ...
    <element-citation publication-type="journal">
         ...
       <article-title>La langue française dans sa diversité.</article-title>
         ...
    </element-citation>
    ...

.. {"reviewed_on": "20180508", "by": "fabio.batalha@erudit.org"}