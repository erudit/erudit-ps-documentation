.. _element-aff:

<aff>
=====

Mandatory attributes:

  1. ``@id`` (ver :ref:`id-attribution-tips`)

Mandatory elements:
 
  1. ``institution[@content-type="orgname"]``

+-------------------------------+--------------------+
| Appears in                    | Frequency          |
+===============================+====================+
| :ref:`element-article-meta`   | Zero or more times |
+-------------------------------+--------------------+

Affiliation data is important for locating and measuring scientific output by country, state, and city, as well as by institution and its departments.

It is recommended that the names of the institutions be used in their original form, not in their translated or abbreviated forms.

When there is more than one form for a name, always use the original one.

Example:

.. code-block:: xml

  ...
  <article-meta>
    ...
    <aff id="aff1">
      <institution content-type="orgname">German Primate Center GmbH</institution>
      <institution content-type="orgdiv1">Neurobiology Laboratory</institution>
      <city>Göttingen</city>
      <country>Germany</country>
    </aff>
    ...
  </article-meta>
  ...


.. {"reviewed_on": "20190411", "by": "fabio.batalha@erudit.org"}
