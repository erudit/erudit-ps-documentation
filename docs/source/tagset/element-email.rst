.. _element-email:

<email>
=======

+-------------------------+--------------------+
| Appears in              | Frequency          |
+=========================+====================+
| :ref:`element-contrib`  | Zero or more times |
+-------------------------+--------------------+
| :ref:`element-aff`      | Zero or more times |
+-------------------------+--------------------+
| :ref:`element-corresp`  | Zero or more times |
+-------------------------+--------------------+

Identifies the e-mail address of the context it is inside.

Examples:

  * :ref:`element-email-example-1`
  * :ref:`element-email-example-2`
  * :ref:`element-email-example-3`

.. _element-email-example-1:

Example of ``<email>`` in ``<contrib>``:
----------------------------------------

.. code-block:: xml

  ...
  <contrib-group content-type="author">
    ...
    <contrib contrib-type="person">
      <contrib-id contrib-id-type="orcid">0000-0003-2125-060X</contrib-id>
      <name>
        <surname>Einstein</surname>
        <given-names>Albert</given-names>
      </name>
      <email>albert@einstein.org</email>
      <xref ref-type="aff" rid="aff1"/>
    </contrib>
    ...
  </contrib-group>
  ...

.. _element-email-example-2:

Example of ``<email>`` in ``<aff>``:
------------------------------------

.. code-block:: xml

  ...
  <article-meta>
    ...
    <aff id="aff01">
        ...
        <email>division@affiliation.com</email>
        ...
    </aff>
    ...
  </article-meta>
  ...

.. _element-email-example-3:

Example of ``<email>`` in ``<corresp>``:
----------------------------------------

.. code-block:: xml

    ...
    <corresp id="c01">
        <label>*</label>
        <italic>E-mail:</italic>
        <email>person@place.com</email>
    </corresp>
    ...


.. {"reviewed_on": "20180523", "by": "fabio.batalha@erudit.org"}
