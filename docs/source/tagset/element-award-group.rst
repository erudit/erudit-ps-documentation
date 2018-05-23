.. _element-award-group:

<award-group>
=============

+-------------------------------+-------------------+
| Appears in                    | Freqency          |
+===============================+===================+
| :ref:`element-funding-group`  | Uma or more times |
+-------------------------------+-------------------+


Identifies a award group with funding information related to the article. There can be as many award groups as funders.

Example:

.. code-block:: xml

  ...
  <fundind-group>
    ...
    <award-group>
      <funding-source>NSERC</funding-source>
      <award-id>24633</award-id>
    </award-group>
    ...
  </funding-group>
  ...


.. {"reviewed_on": "20180423", "by": "fabio.batalha@erudit.org"}
