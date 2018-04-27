.. _element-publisher-loc:

<publisher-loc>
===============

+----------------------------------+--------------------+
| Appears at                       | Frequency          |
+==================================+====================+
| :ref:`element-element-citation`  | Zero or more times |
+----------------------------------+--------------------+
| :ref:`element-product`           | Zero or more times |
+----------------------------------+--------------------+

Identifies the physical location of a publishing house or publisher.


Examples:

  * :ref:`element-pub-name-example-1`
  * :ref:`element-pub-name-example-2`


.. _element-pub-name-example-1:

Example of ``<publisher-loc>`` in ``<journal-meta>``:
-----------------------------------------------------

.. code-block:: xml

    ...
    <publisher>
        <publisher-name>Revue de l'Université de Moncton</publisher-name>
        <publisher-loc>Washington DC</publisher-loc> 
    </publisher>
    ...

.. _element-pub-name-example-2:

Example of ``<publisher-loc>`` in ``<element-citation>``:
---------------------------------------------------------

.. code-block:: xml

    ...
    <element-citation publication-type="book">
        ...
        <publisher-name>National Academy of Science</publisher-name>
        <publisher-loc>Washington DC</publisher-loc>
        ...
    </element-citation>
    ...


.. {"reviewed_on": "201804627", "by": "fabio.batalha@erudit.org"}
