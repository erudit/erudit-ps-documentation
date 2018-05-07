.. _element-date:

<date>
======

Mandatory attributes:

  1. ``@date-type``

+-------------------------+--------------------+
| Appears at              | Frequency          |
+=========================+====================+
| :ref:`element-history`  | Once or more times |
+-------------------------+--------------------+



``<date>`` must have the element :ref:`element-year`. The ``@date-type`` attribute is used to specify the kind of action related to the date.

The allowed values for the attribute ``@date-type`` are:

+-------------+--------------------------------------------------+
| Value       | Description                                      |
+=============+==================================================+
| accepted    | The date the document was accepted               |
+-------------+--------------------------------------------------+
| corrected   | The date the document was corrected              |
+-------------+--------------------------------------------------+
| pub         | Publication date (eletronic or print )           |
+-------------+--------------------------------------------------+
| preprint    | The date the preprint was published              |
+-------------+--------------------------------------------------+
| retracted   | The date the document was retracted              |
+-------------+--------------------------------------------------+
| received    | The date the document was received by the editor |
+-------------+--------------------------------------------------+
| rev-recd    | The date the document was reviewed               |
+-------------+--------------------------------------------------+
| rev-request | The date in which reviews where requested        |
+-------------+--------------------------------------------------+

Example:

.. code-block:: xml

    ...
    <article-meta>
        ...
        <history>
            <date date-type="received">
                <day>15</day>
                <month>03</month>
                <year>2013</year>
            </date>
            <date date-type="rev-recd">
                <day>06</day>
                <month>11</month>
                <year>2013</year>
            </date>
            <date date-type="accepted">
                <day>12</day>
                <month>05</month>
                <year>2014</year>
            </date>
        </history>
        ...
    </article-meta>
    ...


.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}
