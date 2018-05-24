.. _element-institution-id:

<institution-id>
================

+-------------------------+--------------------+
| Appears in              | Frequency          |
+=========================+====================+
| ``<institution-wrap>``  | Zero or more times |
+-------------------------+--------------------+

This element associate an indetifier to an institution declared in the element :ref:`element-aff`.

Exemplo:

.. code-block:: xml

    ...
  ...
  <article-meta>
    ...
    <aff id="aff1">
      <institution content-type="orgname">Université de Moncton</institution>
      <institution-wrap>
        <institution-id institution-id-type="insi">0000 0001 2175 1792</institution-id>
      </institution-wrap>
      <country country="CA">Canada</country>
      <state>NB</state>
      <city>Moncton</city>
    </aff>
    ...
  </article-meta>
  ...

.. {"reviewed_on": "20180524", "by": "fabio.batalha@erudit.org"}