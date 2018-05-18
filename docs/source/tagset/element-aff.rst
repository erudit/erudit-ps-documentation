.. _element-aff:

<aff>
=====

Mandatory attributes:

  1. ``@id`` (ver :ref:`id-attribution-tips`)

+-------------------------------+--------------------+
| Appears in                    | Frequency          |
+===============================+====================+
| :ref:`element-article-meta`   | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-contrib-group`  | Zero or more times |
+-------------------------------+--------------------+
| :ref:`element-front-stub`     | Zero or more times |
+-------------------------------+--------------------+

Used for the article contributors’ institutional affiliation or attachment at the time the article was written, stated either by their degree in process, for example, Masters, Doctorate or Postdoc, etc, or as persons directly affiliated with the institution, for example, Professor at University X, Doctor at institution Y, and Nurse at Hospital Z.

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
      <uri content-type="entity">organisation-1</uri>
    </aff>
    ...
  </article-meta>
  ...


.. {"reviewed_on": "20180518", "by": "fabio.batalha@erudit.org"}
