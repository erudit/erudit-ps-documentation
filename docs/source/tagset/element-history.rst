.. _element-history:

<history>
=========

+------------------------------+------------------+
| Apears in                    | Frequenct        |
+==============================+==================+
| :ref:`element-article-meta ` | Zero or one time |
+------------------------------+------------------+

Groups the dates on which the article was received, accepted and/or reviewed. It must have the elements of type :ref:`element-date`.

Example:

.. code-block:: xml

   ...
   <history>
        <date date-type="received">
             <day>20</day>
             <month>10</month>
             <year>2014</year>
        </date>
        <date date-type="rev-recd">
             <day>06</day>
             <month>12</month>
             <year>2014</year>
        </date>
        <date date-type="accepted">
             <day>14</day>
             <month>07</month>
             <year>2015</year>
        </date>
   </history>
   ...

.. {"reviewed_on": "20180508", "by": "fabio.batalha@erudit.org"}