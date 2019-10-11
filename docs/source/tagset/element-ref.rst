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

This element is used solely to identify references in any format, and describes books, journals, conferences, etc. This element must have one element :ref:`element-mixed-citation` and may also have one element :ref:`element-element-citation`.

.. note::

    * If the reference has a DOI number it must be tagged inside an :ref:`element-element-citation` with the element :ref:`element-pub-id`


Examples:

* :ref:`element-ref-example-1`
* :ref:`element-ref-example-2`

.. _element-ref-example-1:

1. Ref with one :ref:`element-mixed-citation`
---------------------------------------------

.. code-block:: xml

    ...
        <ref-list>
          <ref id="B1">
            <mixed-citation publication-type="journal">
              ...
            </mixed-citation>
          </ref>
          <ref id="B2">
            <mixed-citation publication-type="book">
              ...
            </mixed-citation>
          </ref>
          ...
        </ref-list>
    ...

.. _element-ref-example-2:

2. Ref with one :ref:`element-mixed-citation` and one :ref:`element-element-citation`
-------------------------------------------------------------------------------------
.. code-block:: xml

    ...
        <ref-list>
          <ref id="B1">
            <mixed-citation publication-type="journal">
              ...
            </mixed-citation>
            <element-citation>
              <pub-id pub-id-type="doi">
                  https://doi.org/10.7202/1016689ar
              </pub-id>
            </element-citation>
          </ref>
          <ref id="B2">
            <mixed-citation publication-type="book">
              ...
            </mixed-citation>
          </ref>
          ...
        </ref-list>
    ...


.. {"reviewed_on": "20190910", "by": "mathieu.pigeon@erudit.org"}
