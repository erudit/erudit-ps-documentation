.. _element-month:

<month>
=======

+---------------------------------+------------------+
| Appears in                      | Frequency        |
+=================================+==================+
| :ref:`element-date`             | Zero or one time |
+----------------------------------+-----------------+
| :ref:`element-element-citation` | Zero or one time |
+----------------------------------+-----------------+
| :ref:`element-product`          | Zero or one time |
+----------------------------------+-----------------+
| :ref:`element-pub-date`         | Zero or one time |
+---------------------------------+------------------+

Identifies the month in references or in the front metadata and can represent:

* the month of publication of a scientific journal;
* the month a report is produced;
* the publication month of an article, ver :ref:`element-pub-date` or of a product, see :ref:`element-product` when used in  :ref:`elemento-front`.

The allowed values are whole numbers of up to two digits, between 1 and 12 inclusive.

Month ranges, for example, **Jab - mar** should be identifed in season :ref:`element-season`.

Examples:

  * :ref:`element-month-example-1`
  * :ref:`element-month-example-2`
  * :ref:`element-month-example-3`

.. _elemento-month-exemplo-1:

Example of ``<month>`` in ``<pub-date>``:
-----------------------------------------

.. code-block:: xml

   ...
   <pub-date pub-type="epub-ppub">
        <day>01</day>
        <month>06</month>
        <year>2016</year>
   </pub-date>
   ...

.. _element-month-example-2:

Example of ``<month>`` in ``<date>`` of ``<history>``:
------------------------------------------------------

.. code-block:: xml

    ...
    <history>
      <date date-type="received">
        <day>20</day>
        <month>10</month>
        <year>2014</year>
      </date>
    </history>
    ...

.. _element-month-example-3:

Example of ``<month>`` in ``<element-citation>``:
-------------------------------------------------

.. code-block:: xml

   ...
   <element-citation publication-type="book">
        <person-group person-group-type="author">
             <collab>American Occupational Therapy Association, Ad Hoc Committee on Occupational Therapy Manpower</collab>
        </person-group>
        <source>Occupational therapy manpower: a plan for progress</source>
        <publisher-loc>Rockville (MD)</publisher-loc>
        <publisher-name>The Association</publisher-name>
        <year>1985</year>
        <month>4</month>
        <size units="page">84 p</size>
   </element-citation>
   ...

.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}