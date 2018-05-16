.. _element-name:

<name>
======

+------------------------------+--------------------+
| Appears in                   | Frequency          |
+==============================+====================+
| :ref:`element-contrib`       | Zero or once       |
+------------------------------+--------------------+
| :ref:`element-person-group`  | Zero or more times |
+------------------------------+--------------------+

The element ``<name>`` is used to specify the personal name of a contributing author. The possible elements in ``<name>`` are: :ref:`element-surname`,:ref:`element-given-names`, :ref:`element-prefix`, :ref:`element-suffix`, and must be used in this same sequence.

Examples:

  * :ref:`element-name-example-1`
  * :ref:`element-name-example-2`


.. _element-name-example-1:

Example of ``<name>`` in ``<contrib>``:
---------------------------------------

.. code-block:: xml

  ...
  <contrib-group contrib-type="author">
    ...
    <contrib contrib-type="person">
      <name>
        <surname>Amon</surname>
        <given-names>Joseph J.</given-names>
      </name>
    </contrib>
    ...
  </contrib-group>
  ...


.. _element-name-example-2:

Example of ``<name>`` in ``<person-group>``:
--------------------------------------------

.. code-block:: xml

 ...
  <contrib-group contrib-type="author">
    ...
    <person-group person-group-type="person">
      <name>
        <surname>Silva</surname>
        <given-names>Jaqueline Figueiredo da</given-names>
      </name>
    </person-group>
    ...
  </contrib-group>
  ...

.. {"reviewed_on": "20180516", "by": "fabio.batalha@erudit.org"}