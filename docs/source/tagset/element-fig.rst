.. _element-fig:

<fig>
=====


Mandatory attributes:

  1. ``@id`` (see :ref:`id-attribution-tips`)

+-------------------------------------------+--------------------+
| Appears in                                | Frequency          |
+===========================================+====================+
| :ref:`element-app`                        | Zero or more times |
+-------------------------------------------+--------------------+
| :ref:`element-body`                       | Zero or more times |
+-------------------------------------------+--------------------+
| ``<fig-group>``                           | Zero or more times |
+-------------------------------------------+--------------------+
| :ref:`element-glossary`                   | Zero or more times |
+-------------------------------------------+--------------------+
| :ref:`element-p`                          | Zero or more times |
+-------------------------------------------+--------------------+
| :ref:`element-supplementary-material`     | Zero or more times |
+-------------------------------------------+--------------------+
| other elements see JATS Spec for details  | Zero or more times |
+-------------------------------------------+--------------------+

Identifies the figures in an article. In this element you must specify the element :ref:`element-label`, you can also specify the elements :ref:`element-caption`, ``<graphic>`` e :ref:`permissions`. ``<fig>`` can still have the following attributes: ``@fig-type`` and ``@xml:lang``.

The ``<graphic>`` element is used to identify some file types and has attribute ``@xlink:href`` which is used to specify the complete name of the referenced image.

The attribute ``@id`` allows for cross-referencing within the document (link associated with an “rid”) provided that the attribute has a unique value within the file.

Examples:

    * :ref:`element-fig-example-1`
    * :ref:`element-fig-example-2`
    * :ref:`element-fig-example-3`
    * :ref:`element-fig-example-4`
    * :ref:`element-fig-example-5`

.. _element-fig-example-1:

Example of figure without caption:
----------------------------------

The figures may or may not have captions. Figures without a caption should be marked  as ``<fig>`` and identified with the element ``<graphic>``.

.. code-block:: xml

  ...
  <fig id="f1">
    <label>Fig. 1</label>
    <graphic xlink:href="figure.tif"/>
  </fig>
  ...


.. _element-fig-example-2:

Example of figue with caption:
------------------------------

.. code-block:: xml

  ...
  <fig id="f03">
    <label>Fig. 3</label>
    <caption>
      <title>Figure Title</title>
    </caption>
    <graphic xlink:href="figure.tif"/>
  </fig>
  ...


.. _element-fig-example-3:

Example of figure with custom @fig-type:
----------------------------------------

The attribute ``@fig-type`` is used to specify the image type, the value could be one of:

+--------------+
| Value        |
+==============+
| graphic      |
+--------------+
| chart        |
+--------------+
| diagram      |
+--------------+
| drawing      |
+--------------+
| illustration |
+--------------+
| map          |
+--------------+

Be sure to represent the correct :ref:`elemento-label` accoding to the ``@fig-type``.

.. code-block:: xml

  ...
  <fig fig-type="map" id="f1">
    <label>Map 1</label>
    <caption>
      <title>Map Title<title>
    </caption>
    <graphic xlink:href="figure.tif"/>
  </fig>
  ...

.. _element-fig-example-4:

Example of figure with permissions or source information:
---------------------------------------------------------

.. code-block:: xml

  ...
  <fig id="f1">
    <label>Fig. 1</label>
    <caption>
      <title>Deaths among patients receiving day hospital care or alternative services.</title>
      <p>Odds ratios of death by end of follow up were calculated by fixed effects model. Heterogeneity between trials is presented as &#x03C7;<sup>2</sup></p>
    </caption>
    <permissions>
      <copyright-statement>Source: The National Portrait Gallery, London. All rights reserved</copyright-statement>
      <copyright-year>2013</copyright-year>
    </permissions>
    <graphic xlink:href="fig.tif" />
  </fig>
  ...


.. _elemento-fig-exemplo-5:

Example of figure with translated caption:
------------------------------------------

Figures that have translated captions (have more than one :ref:`label` and :ref:`caption` must be identified with the element ``<fig-group>`` which must contain a ``<fig>`` element for each language, as well as the attribute ``@xml:lang``.

.. code-block:: xml

    ...
    <fig-group id="f1">
        <fig xml:lang="pt">
            <label>Figura 1</label>
            <caption>
                <title>Caracterização química em óxidos do rejeito.</title>
            </caption>
        </fig>
        <fig xml:lang="en">
            <label>Figure 1</label>
            <caption>
                <title>Chemical characterization of the oxides of the tailing.</title>
            </caption>
        </fig>
        <graphic xlink:href="figure.tif"/>
    </fig-group>
    ...


.. {"reviewed_on": "20180528", "by": "fabio.batalha@erudit.org"}
