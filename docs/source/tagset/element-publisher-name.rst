.. _element-publisher-name:

<publisher-name>
================

+----------------------------------+--------------------+
| Appears at                       | Fequency           |
+==================================+====================+
| :ref:`element-element-citation`  | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-product`           | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-publisher`         | Zero or more times |
+----------------------------------+--------------------+

Represents the name of the publishing house or publisher.

Examples:

  * :ref:`element-pub-name-exemplo-1`
  * :ref:`element-pub-name-exemplo-2`


.. _element-pub-name-exemplo-1:

Example of ``<publisher-name>`` in ``<journal-meta>``:
------------------------------------------------------

.. code-block:: xml

    ...
    <publisher>
        <publisher-name>Revue de l'Université de Moncton</publisher-name>
    </publisher>
    ...

.. _element-pub-name-exemplo-2:

Example of ``<publisher-name>`` in ``<element-citation>``:
----------------------------------------------------------

.. code-block:: xml

    ...
    <element-citation publication-type="book">
               ...
        <publisher-name>Revue de l'Université de Moncton</publisher-name>
        <fpage>223</fpage>
        <lpage>244</lpage>
    </element-citation>
    ...


.. {"reviewed_on": "201804627", "by": "fabio.batalha@erudit.org"}
