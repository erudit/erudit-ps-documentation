.. _element-permissions:

<permissions>
=============

+----------------------------------------+--------------------+
| Appears in                             | Frequency          |
+========================================+====================+
| :ref:`element-article-meta`            | Once               |
+----------------------------------------+--------------------+
| :ref:`element-boxed-text`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-disp-quote`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-fig`                     | Zero or more times |
+----------------------------------------+--------------------+
| ``<graphic>``                          | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-media`                   | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-supplementary-material`  | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-table-wrap`              | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-verse-group`             | Zero or more times |
+----------------------------------------+--------------------+

Permissions are a set of conditions under which article content can be used, accessed, and distributed.

The table below shows the type of object in a text, the elements which can have ``<permissions>``, and what is included in the ``<permissions>``.

+--------------------------+---------------------------------------+
| Elements that can have   | What the permission includes          |
| ``<permisssions>``       |                                       |
+==========================+=======================================+
| <boxed-text>             | The element itself                    |
+--------------------------+---------------------------------------+
| <disp-quote>             | The element itself                    |
+--------------------------+---------------------------------------+
| <fig>                    | All figure and related files          |
+--------------------------+---------------------------------------+
| <graphic>                | The image file (`@xlink:href`) and    |
|                          | its description                       |
+--------------------------+---------------------------------------+
| <media>                  | The image file (`@xlink:href`) and    |
|                          | its description                       |
+--------------------------+---------------------------------------+
| <supplementary-material> | The file of supplementary material    |
|                          | and its description                   |
+--------------------------+---------------------------------------+
| <table-wrap>             | The table, the label, caption, and    |
|                          | table footnotes                       |
+--------------------------+---------------------------------------+
| <verse-group>            | The element itself                    |
+--------------------------+---------------------------------------+

.. note::

  Read `JATS4R rules <https://jats4r.org/permissions>`_ for best practive to use the ``<permissions>`` element.

Examples:

  * :ref:`element-permissions-example-1`
  * :ref:`element-permissions-example-2`
  * :ref:`element-permissions-example-3`
  * :ref:`element-permissions-example-4`

.. _element-permissions-example-1:

1. Article use license ``<article-meta>``
-----------------------------------------

.. code-block:: xml

    ...
    <article-meta>
      ...
      <permissions>
        <copyright-statement>Tous droits réservés © Revue de l’Université de Moncton</copyright-statement>
        <copyright-year>2015</copyright-year>
        <copyright-holder>Revue de l’Université de Moncton</copyright-holder>
        <license>
          <license-p>Tous droits réservés © Revue de l’Université de Moncton, 2015</license-p>
        </license>
      </permissions>
      ...
    </article-meta>
    ...


.. _element-permissions-example-2:

2. Credits of a figure ``<fig>``
--------------------------------

.. code-block:: xml

    ...
    <fig id="f01">
      <label>Figure 1</label>
      <caption>
        <title>The classic regular poutine: fries, cheese curds and brown gravy.</title>
      </caption>
      <graphic xlink:href="image.tif"/>
      <permissions>
        <license xml:lang="en">
          <license-p>Photographic credit: La Poutine Week</license-p>
        </license>
      </permissions>
    </fig>
    ...


.. _element-permissions-example-3:

3. Credits in ``<table-wrap>``
------------------------------

.. code-block:: xml

   ...
   <table-wrap>
    <label>Table 1</label>
    <caption>
      <title>Chemical characterization of the oxides of the tailing</title>
    </caption>
    <table frame="hsides" rules="groups">
     <thead>
        <tr>
          <th>Variable</th>
          <th>Results (N=880)</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <td align="center">Gender</td>
          <td align="center"/>
        </tr>
        <tr>
          <td align="center">Male</td>
          <td align="center">411 (46,7)</td>
        </tr>
        <tr>
          <td align="center">Female</td>
          <td align="center">469 (53,3)</td>
        </tr>
      </tbody>
    </table>
    <permissions>
      <copyright-statement>Copyright © 2014 Érudit</copyright-statement>
      <copyright-year>2014</copyright-year>
      <copyright-holder>Érudit</copyright-holder>
      <license license-type="open-access" xlink:href="http://creativecommons.org/licenses/by-nc-sa/4.0/" xml:lang="en">
        <license-p>This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.</license-p>
      </license>
    </permissions>
   </table-wrap>

.. _element-permissions-example-4:

4. Refers to a table as image in ``<table-wrap>``
-------------------------------------------------

.. code-block:: xml

   ...
   <table-wrap>
    <label>Table 3</label>
    <caption>
      <title>Multivariate analysis of risk factors associated with readmission - Model 2</title>
    </caption>
    <graphic xlink:href="image.tif"/>
    <permissions>
      <copyright-statement>Copyright © 2014 Érudit</copyright-statement>
      <copyright-year>2014</copyright-year>
      <copyright-holder>Érudit</copyright-holder>
      <license license-type="open-access" xlink:href="http://creativecommons.org/licenses/by-nc-sa/4.0/" xml:lang="en">
        <license-p>This work is licensed under a Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License.</license-p>
      </license>
    </permissions>
 </table-wrap>

.. {"reviewed_on": "20180515", "by": "fabio.batalha@erudit.org"}