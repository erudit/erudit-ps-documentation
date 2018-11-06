.. _element-string-name:

<string-name>
=============

+-------------------------+--------------------+
| Appears in              | Frequency          |
+=========================+====================+
| :ref:`element-contrib`  | Zero or more times |
+-------------------------+--------------------+

Identifies an alternative name for the author.

Examples:

  * :ref:`element-string-name-example-1`

.. _element-string-name-example-1:

Example of ``<string-name>`` in ``<contrib>``:
----------------------------------------------

.. code-block:: xml

  ...
  <contrib-group content-type="author">
    ...
    <contrib contrib-type="person">
      ...
      <name>
        <surname>Tuch</surname>
        <given-names>Kurt</given-names>
      </name>
      <string-name content-type="alias">Panter Pan<string-name>
      <email>kurt@tuch.org</email>
      ...
    </contrib>
    ...
  </contrib-group>
  ..

.. {"reviewed_on": "20181106", "by": "fabio.batalha@erudit.org"}
