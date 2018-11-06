.. _element-bio:

<bio>
=============

+-------------------------+--------------------+
| Appears in              | Frequency          |
+=========================+====================+
| :ref:`element-contrib`  | Zero or more times |
+-------------------------+--------------------+

Author biography.

Example:

.. code-block:: xml

  ...
  <contrib-group content-type="author">
    ...
    <contrib contrib-type="person">
      ...
      <name>
        <surname>Cabot</surname>
        <given-names>John</given-names>
      </name>
      <bio>
        <p>John Doe is the head of the department of ...</p>
      </bio>
      <email>john@cabot.org</email>
      ...
    </contrib>
    ...
  </contrib-group>
  ..

.. {"reviewed_on": "20181106", "by": "fabio.batalha@erudit.org"}
