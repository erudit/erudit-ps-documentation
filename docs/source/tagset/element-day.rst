.. _element-day:

<day>
=====

+----------------------------------+------------------+
| Appears in                       | Frequency        |
+==================================+==================+
| :ref:`element-pub-date`          | Zero or one time |
+----------------------------------+------------------+
| :ref:`element-product`           | Zero or one time |
+----------------------------------+------------------+
| :ref:`element-element-citation`  | Zero or one time |
+----------------------------------+------------------+
| :ref:`element-date-in-citation`  | Zero or one time |
+----------------------------------+------------------+
| :ref:`element-date`              | Zero or one time |
+----------------------------------+------------------+

Identifies the day of a date, it could be:

 * The date of publication of the document in :ref:`article-meta`
 * The date of publication of the document in :ref:`element-citation`
 * the date of access to a website link in a reference

This element have a value up to 2 numeric digits.

Example:

.. code-block:: xml

    ...
    <day>12</day>
    ...


.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}
