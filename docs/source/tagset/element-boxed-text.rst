.. _element-boxed-text:

<boxed-text>
============

Mandatory attributes:

  1. ``@id`` (ver :ref:`id-attribution-tips`)

+----------------------------+--------------------+
| Appears in                 | Frequency          |
+============================+====================+
| :ref:`element-app`         | Zero or more times |
+----------------------------+--------------------+
| ``<app-group>``            | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-body`        | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-boxed-text`  | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-glossary`    | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-p`           | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-ref-list`    | Zero or more times |
+----------------------------+--------------------+
| :ref:`element-sec`         | Zero or more times |
+----------------------------+--------------------+

This element identifies texts inserted in a box. Allows for the presentation of text with sections, figures, tables, etc

Examples:

  * :ref:`element-boxtext-example-1`
  * :ref:`element-boxtext-example-2`

.. _element-boxtext-example-1:

Exemple of ``<boxed-text>`` with section:
-----------------------------------------

.. code-block:: xml

    ...
    <boxed-text id="bx1">
        <sec>
            <title>Box 1 Use of antidepressants and suicidality in young individuals</title>
            <p>In 2004, the FDA made the decision to include a black box warning about the risk of suicidality associated with antidepressant use among individuals under 25 years of age<xref ref-type="bibr" rid="B26">26</xref>.</p>
            <p>Based on the fact that for the treatment of depressive disorders the number needed to treat (NNT) in this age group is at least 10 and the number needed to harm (number needed to harm, NNH) is 112, it was concluded that the benefits associated with the use of antidepressants outweigh the potential risks.</p>
        </sec>
    </boxed-text>
    ...

.. _element-boxtext-example-2:

Example of ``<boxed-text>`` with  figure:
-----------------------------------------

.. code-block:: xml

    ...
    <boxed-text id="bx1">
        <fig id="f12">
            <label>Figure</label>
            <caption>
                <title>Diagnostic algorithm for depressive episodes in children and adolescents</title>
            </caption>
            <graphic xlink:href="figure.jpg"/>
        </fig>
    </boxed-text>
    ...

.. {"reviewed_on": "20180603", "by": "fabio.batalha@erudit.org"}
