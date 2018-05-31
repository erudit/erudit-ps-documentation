.. _element-season:

<season>
========

+----------------------------------+-----------------+
| Appears in                       | Frequency       |
+==================================+=================+
| :ref:`element-element-citation` | Zero or one time |
+----------------------------------+-----------------+
| :ref:`element-product`          | Zero or one time |
+----------------------------------+-----------------+
| :ref:`element-pub-date`         | Zero or one time |
+----------------------------------+-----------------+

This element can occur in :ref:`pub-date` to identify a month range (see Note below), and in :ref:`element-citation` and :ref:`product` to identify the season in a bibliographic reference.

As a pattern Érudit PS have a list of valid values for seasons. These values are not mandatory in this version of Érudit PS, but have in mind to follow these best practices to be under conformit with the next versions of Érudit PS.

List of known seasons:

+---------------+
| value         |
+===============+
| spring        |
+---------------+
| summer        |
+---------------+
| outumn        |
+---------------+
| winter        |
+---------------+
| January       |
+---------------+
| Februrary     |
+---------------+
| March         |
+---------------+
| April         |
+---------------+
| May           |
+---------------+
| June          |
+---------------+
| July          |
+---------------+
| August        |
+---------------+
| September     |
+---------------+
| October       |
+---------------+
| November      |
+---------------+
| December      |
+---------------+
| Christmas     |
+---------------+
| 1st quarter   |
+---------------+
| 2nd quarter   |
+---------------+
| 3th quarter   |
+---------------+
| 4th quarter   |
+---------------+
| 1st semester  |
+---------------+
| 2nd semester  |
+---------------+

.. note::

    An hyphen must be used to combine more than one season, ex: may-june, spring-summer, etc.


Examples:

    * :ref:`element-season-example-1`
    * :ref:`element-season-example-2`
    * :ref:`element-season-example-3`


.. _element-season-example-1:

Example of ``<season>`` as a season:
------------------------------------

.. code-block:: xml

    ...
    <back>
        ...
        <ref-list>
            <ref>
                ...
                <season>Autumn</season>
                ...
            </ref>
        </ref-list>
        ...
    </back>


.. _element-season-example-2:

Example ``<season>`` as a month range:
--------------------------------------

.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <pub-date pub-type="epub">
                <season>Nov-Dec</season>
                <year>2013</year>
            </pub-date>
            ...
        </article-meta>
        ...
    </front>
    ...

.. _element-season-example-3:

Example ``<season>`` as a season range:
---------------------------------------

.. code-block:: xml

    ...
    <front>
        ...
        <article-meta>
            ...
            <pub-date pub-type="epub">
                <season>spring-summer</season>
                <year>2013</year>
            </pub-date>
            ...
        </article-meta>
        ...
    </front>
    ...

.. {"reviewed_on": "20180507", "by": "fabio.batalha@erudit.org"}