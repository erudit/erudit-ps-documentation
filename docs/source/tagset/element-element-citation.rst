.. _element-element-citation:

<element-citation>
==================

+---------------------+--------------------+
| Appears in          | Frequency          |
+=====================+====================+
| :ref:`element-ref`  | Zero or once       |
+---------------------+--------------------+

``<element-citation>`` is used in :ref:`element-ref` to identify the DOI of the cited reference when it is available. This element may also be used to provide a detailed identification of a bibliographic reference. If so, it content must comply to the `JATS 1.2 standard <https://jats.nlm.nih.gov/archiving/tag-library/1.2/element/element-citation.html>`_.

.. note::

    For compatibility with ``Érudit Article`` see :ref:`compatibility-reference` section.

Examples:

  * :ref:`element-element-citation-example-1`
  * :ref:`element-element-citation-example-2`

.. _element-element-citation-example-1:

1. Mixed-citation and element-citation (DOI only)
-------------------------------------------------

.. code-block:: xml

    <!-- Journal Sample -->

    ...
    <ref-list>
      <ref id="B1">
        <mixed-citation publication-type="journal">
            Arrighi, L. et Boudreau, A. (2013). La construction discursive de l'identité francophone en Acadie ou «comment être francophone à partir des marges?». Minorités linguistiques et société/Linguistic Minorities and Society. 2. 8-92.
        </mixed-citation>
        <element-citation>
          <pub-id pub-id-type="doi">
              https://doi.org/10.7202/1016689ar
          </pub-id>
        </element-citation>
      </ref>
    <ref-list>
    ...

.. _element-element-citation-example-2:

2. Mixed-citation and detailed element-citation
------------------------------------------------

.. code-block:: xml

    <!-- Journal Sample -->

    ...
    <ref-list>
      <ref id="B1">
        <mixed-citation publication-type="journal">
            Arrighi, L. et Boudreau, A. (2013). La construction discursive de l'identité francophone en Acadie ou «comment être francophone à partir des marges?». Minorités linguistiques et société/Linguistic Minorities and Society. 2. 8-92.
        </mixed-citation>
        <element-citation>
        <person-group person-group-type="author">
            <name>
              <surname>
                  Arrighi
              </surname>
              <given-names>
                  L.
              </given-names>
            </name>
            <name>
              <surname>
                  Boudreau
              </surname>
              <given-names>
                  A.
              </given-names>
            </name>
          </person-group>
          <year>
              2013
          </year>
          <source>
              Minorités linguistiques et société
          </source>
            <article-title>
                La construction discursive de l'identité francophone en Acadie ou «comment être francophone à partir des marges?»
            </article-title>
          <issue>
              2
          </issue>
          <fpage>
              8
          </fpage>
          <lpage>
              92
          </lpage>
          <pub-id pub-id-type="doi">
              https://doi.org/10.7202/1016689ar
          </pub-id>
        </element-citation>
      </ref>
    <ref-list>
    ...







.. {"reviewed_on": "20190911", "by": "mathieu.pigeon@erudit.org"}
