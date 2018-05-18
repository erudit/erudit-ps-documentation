.. _element-institution:

<institution>
=============

Mandatory attributes:

  1. ``@content-type``

+---------------------+--------------------+
| Appears in          | Frequency          |
+=====================+====================+
| :ref:`element-aff`  | One or more times  |
+---------------------+--------------------+

This element identifies the author’s institutional affiliation which can be divided into up to three levels as defined by the mandatory attribute ``@content-type`` whose possible values are:

+------------+--------------------------------------------------------------------+
| Value      | Description                                                        |
+============+====================================================================+
| orgname    | Represents the first (highest) level of a multi-tier institution   |
|            | mentioned in the affiliation.                                      |
+------------+--------------------------------------------------------------------+
| orgdiv1    | Represents the first subdivision of the institution mentioned.     |
|            |                                                                    |
+------------+--------------------------------------------------------------------+
| orgdiv2    | Represents the second subdivision of the institution mentioned.    |
|            |                                                                    |
+------------+--------------------------------------------------------------------+
| original   | Identifies the complete affiliation as it appears in the text of   |
|            | the document.                                                      |
+------------+--------------------------------------------------------------------+

.. note:: 
 * Divisions below the third hierarchique level must be identified in the element ``<institution content-type="original">``.

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


Example of ``content-type='original'``:

.. code-block:: xml

  ...
  <article-meta>
    ...
    <aff id="aff1">
      ...
      <institution content-type="original">
        Técnica de Cardiopneumologia. Unidade de Fisiopatologia Respiratória, Serviço de Pneumologia, Centro Hospitalar Lisboa Norte, Lisboa, Portugal.
      </institution>
    </aff>
    ...
  </article-meta>
  ...
