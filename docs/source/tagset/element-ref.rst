.. _element-ref:

<ref>
=====

Mandatory attributes:

  1. ``@id`` (see :ref:`id-attribution-suggestion`)

+--------------------------+-------------------+
| Appears in               | Frequency         |
+==========================+===================+
| :ref:`element-ref-list`  | One or more times |
+--------------------------+-------------------+

This element is used solely to identify references in any format, and describes books, journals, conferences, etc. This element must have one element :ref:`element-element-citation`.

Exemplo:

.. code-block:: xml

    ...
        <ref-list>
          <ref id="B1">
            <element-citation publication-type="journal">
              ...
            </element-citation>
          </ref>
          <ref id="B2">
            <element-citation publication-type="book">
              ...
            </element-citation>
          </ref>
          ...
        </ref-list>
    ...


.. {"reviewed_on": "20180501", "by": "fabio.batalha@erudit.org"}