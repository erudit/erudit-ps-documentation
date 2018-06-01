.. _element-table-wrap-foot:

<table-wrap-foot>
=================

+----------------------------+--------------------+
| Appears in                 | Frequency          |
+============================+====================+
| :ref:`element-table-wrap`  | Zero or more times |
+----------------------------+--------------------+

The element ``<table-wrap-foot>`` allows for the identification of a table footnote with elements of the type ``<fn>``.

A footnote may be related to information in the body of the table.

Example:

.. code-block:: xml

    ...
    <table-wrap id="t01">
        <label>Table 1</label>
        <caption>
            <title>Table title.</title>
        </caption>
        <table>
            ...
        </table>
        <table-wrap-foot>
            <fn id="TFN01">
                <label>*</label>
                <p>text</p>
            </fn>
        </table-wrap-foot>
    </table-wrap>
    ...

.. {"reviewed_on": "20180601", "by": "fabio.batalha@erudit.org"}
