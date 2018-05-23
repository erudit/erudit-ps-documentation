.. _element-funding-source:

<funding-source>
================

+-----------------------------+-------------------+
| Appears in                  | Frequency         |
+=============================+===================+
| :ref:`element-award-group`  | One or more times |
+-----------------------------+-------------------+

Element contained in :ref:`element-award-group` where the funding entity and/or funding institution, if any, are specified.

Examples:

  * :ref:`element-fundingsource-example-1`
  * :ref:`element-fundingsource-example-2`


.. _element-fundingsource-example-1:

Example of one ``<funding-source>`` for one ``<award-id>`` :
------------------------------------------------------------

.. code-block:: xml

  ...
  <article-meta>
    ...
    <funding-group>
      <award-group>
        <funding-source>NSERC</funding-source>
        <award-id>1685X6</award-id>
      </award-group>
      ...
    </funding-group>
    ...
  </article-meta>
  ...



.. _element-fundingsource-example-2:

Example of two ``<funding-source>`` for one ``<award-id>`` :
------------------------------------------------------------

.. code-block:: xml

  ...
  <article-meta>
   ...
   <funding-group>
      <award-group>
        <funding-source>NSERC</funding-source>
        <funding-source>NCE</funding-source>
        <award-id>06953</award-id>
      </award-group>
      ...
   </funding-group>
   ...
  </article-meta>
  ...


.. {"reviewed_on": "20180523", "by": "fabio.batalha@erudit.org"}
