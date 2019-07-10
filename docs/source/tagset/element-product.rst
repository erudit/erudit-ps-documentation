.. _element-product:

<product>
=========

+----------------------------------+------------------+
| Appears in                       | Frequency        |
+==================================+==================+
| :ref:`element-article-meta`      | Zero or one time |
+----------------------------------+------------------+

Used in :ref:`element-article-meta` to identify the title of a reviewed resource.

Usually review articles don't have :ref:`element-article-title` or :ref:`element-subtitle`.

Consequently they usualy don't have :ref:`element-title-group`. 

.. info::

  Ex: A book review article should have the element product with the title of the
  reviewed book

Examples:

  * :ref:`element-product-example-1`
  * :ref:`element-product-example-2`

.. _element-product-example-1:

Example of ``<product>`` in :ref:`element-article-meta`:
--------------------------------------------------------

.. code-block:: xml

    ...
    <article-meta>
      ...
      <product product-type="book">
          <related-object>Rosa Bruno-Jofré &amp; James Scott Johnston (Eds.). <italic>Teacher Education in a Transnational World</italic>. Toronto, ON: University of Toronto Press. (2014). 466 pp. $75.00 (hardcover). (ISBN 978-1-4426-4934-7)</related-object>
      </product>
      ...
    </article-meta>
    ...

.. _element-product-example-2:

Example of ``<product>`` combined with article-title and subtitle :ref:`element-article-meta`:
----------------------------------------------------------------------------------------------

.. code-block:: xml

    ...
    <article-meta>
      ...
      <title-group>
        <article-title>Romance nouveau genre</article-title>
        <subtitle>Comentaire Critique</subtitle>
      </title-group>
      <product product-type="film">
          <related-object><italique>Les Combattants</italique> de Thomas Cailley, France, 2014, 98 min</related-object>
      </product>
      ...
    </article-meta>
    ...


.. {"reviewed_on": "20190710", "by": "fabio.batalha@erudit.org"}