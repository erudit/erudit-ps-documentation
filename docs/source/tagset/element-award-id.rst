.. _element-award-id:

<award-id>
==========

+-----------------------------+--------------------+
| Appears in                  | Frequency          |
+=============================+====================+
| :ref:`element-award-group`  | Zero or more times |
+-----------------------------+------------------ -+

Specifies the award number given by the funding institution.

Example:

.. code-block:: xml

  ...
  <article-meta>
    ...
    <funding-group>
      <award-group>
        <funding-source>NSERC</funding-source>
        <award-id>24633</award-id>
      </award-group>
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
