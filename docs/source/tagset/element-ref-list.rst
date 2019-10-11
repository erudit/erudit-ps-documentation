.. _element-ref-list:

<ref-list>
==========

+--------------------------+--------------------+
| Appears in               | Frquency           |
+==========================+====================+
| :ref:`element-back`      | Zero or more times |
+--------------------------+--------------------+


Represents the group of bibliographic references in an article, and must contain the
element :ref:`element-ref` which, in turn, must contains the element :ref:`element-mixed-citation` and may contains the element :ref:`element-element-citation`.

In ``<ref-list>``, a title could be inserted using the element ``<title>``.

.. _element-ref-list-example-1:

Example of a simple ``<ref-list>``:
-----------------------------------

.. code-block:: xml

    ...
    <ref-list>
        <title>Bibliographic References</title>
        <ref id="B1">
            ...
        </ref>
        <ref id="B2">
            ...
        </ref>
        ...
    </ref-list>
    ...


.. {"reviewed_on": "20190910", "by": "mathieu.pigeon@erudit.org"}
