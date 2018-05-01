.. _element-ref-list:

<ref-list>
==========

+--------------------------+--------------------+
| Appears in               | Frquency           |
+==========================+====================+
| :ref:`element-back`      | Zero or more times |
+--------------------------+--------------------+


Represents the group of bibliographic references in an article, and must contain the
element :ref:`element-ref` which, in turn, contains the element :ref:`element-element-citation`.

In ``<ref-list>``, a label should could inserted using the element ``<title>`` identifying the section of the text.

.. _element-ref-list-example-1:

Example of a simple ``<ref-list>``:
-----------------------------------

.. code-block:: xml

    ...
    <ref-list>
        <title>Bibliographic References</title>
        <ref id="R1">
            ...
        </ref>
        <ref id="R2">
            ...
        </ref>
        ...
    </ref-list>
    ...


