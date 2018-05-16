.. _element-xref:

<xref>
======

Mandatory attributes:

  1. ``@rid``
  2. ``@ref-type``

+--------------------------------+--------------------+
| Appears in                     | Frequency          |
+================================+====================+
| :ref:`element-article-title`   | Zero or more times |
+--------------------------------+--------------------+
| :ref:`element-attrib`          | Zero or more times |
+--------------------------------+--------------------+
| :ref:`element-contrib`         | Zero or more times |
+--------------------------------+--------------------+
| :ref:`element-p`               | Zero or more times |
+--------------------------------+--------------------+
| ``<td>``                       | Zero or more times |
+--------------------------------+--------------------+
| ``<th>``                       | Zero or more times |
+--------------------------------+--------------------+
| :ref:`element-trans-title`     | Zero or more times |
+--------------------------------+--------------------+
| :ref:`element-sec`             | Zero or more times |
+--------------------------------+--------------------+
| ``<verse-line>``               | Zero or more times |
+--------------------------------+--------------------+

Cross-reference element used to relate and/or create a link with information in the text. The mandatory attributes for xref are:

* ``@rid``: contains the element identifier of the referenced article, thus making the link between the origin (``@rid``) and destination (``@id``) in the text.
* ``@ref-type``: specifies the type of cross-reference whose values can be:

+------------------------+-----------------------------------------+
| Value                  | Description                             |
+========================+=========================================+
| aff                    | affiliation                             |
+------------------------+-----------------------------------------+
| app                    | appendix                                |
+------------------------+-----------------------------------------+
| author-notes           | authors notes                           |
+------------------------+-----------------------------------------+
| bibr                   | bibliographic references                |
+------------------------+-----------------------------------------+
| boxed-text             | text box                                |
+------------------------+-----------------------------------------+
| contrib                | contributor                             |
+------------------------+-----------------------------------------+
| corresp                | corresponding author                    |
+------------------------+-----------------------------------------+
| disp-formula           | formula                                 |
+------------------------+-----------------------------------------+
| fig                    | figura or figure group                  |
+------------------------+-----------------------------------------+
| fn                     | footnotes                               |
+------------------------+-----------------------------------------+
| sec                    | section                                 |
+------------------------+-----------------------------------------+
| supplementary-material | supplementary material                  |
+------------------------+-----------------------------------------+
| table                  | table or table group                    |
+------------------------+-----------------------------------------+
| table-fn               | table footnotes                         |
+------------------------+-----------------------------------------+


Examples:

  * :ref:`element-xref-example-1`
  * :ref:`element-xref-example-2`
  * :ref:`element-xref-example-3`
  * :ref:`element-xref-example-4`


.. _element-xref-example-1:

Example of ``<xref>`` in ``<article-meta>``:
--------------------------------------------

.. code-block:: xml

    ...
    <article-meta>
        ...
        <contrib-group>
            <contrib contrib-type="author">
                <name>
                    <surname>Lacerda</surname>
                    <given-names>Marcus Vale</given-names>
                </name>
                <xref ref-type="aff" rid="aff1">1</xref>
            </contrib>
            <aff id="aff1">
                <label>1</label>
                <institution content-type="orgname">Universidade do Estado do Amazonas</institution>
                <country country="BR">Brazil</country>
                <institution content-type="original">Universidade do Estado do Amazonas, Manaus, AM, Brasil</institution>
            </aff>
            ...
        </contrib-group>
        ...
    </article-meta>
    ...


.. _element-xref-example-2:

Example of ``<xref>`` in ``<p>``:
---------------------------------

.. code-block:: xml

  ...
  <p>
    ...
     <xref ref-type="bibr" rid="B13">John 2003</xref>
     ...
  </p>
  ...


.. _element-xref-example-3:

Example of ``<xref>`` related to a figure in the text:
------------------------------------------------------

.. code-block:: xml

    <p>Check in <xref ref-type="fig" rid="f01">Figure 1</xref></p>
    ...
    <p>
        <fig id="f01">
            <caption>
                <title>Environmental <italic>in situ</italic> conditions during the study period.</title>
            </caption>
            <graphic xlink:href="image.tif"/>
        </fig>
    </p>



.. _element-xref-example-4:

Example ``<xref>`` without content:
-----------------------------------

.. code-block:: xml

  ...
  <article-meta>
    ...
    <contrib-group>
      <contrib contrib-type="author">
        <name>
            <surname>Broering</surname>
            <given-names>Laurent Wiliam</given-names>
        </name>
        <xref ref-type="aff" rid="aff1"/>
      </contrib>
    </contrib-group>
    <aff id="aff1">
      <institution>Fundação Getúlio Vargas</institution>
      <institution content-type="orgdiv1">EAESP</institution>
      <country country="BR">Brazil</country>
      <institution content-type="original">Fundação Getúlio Vargas - FGV-EAESP, Av. 9 de Julho, 2029, Bela Vista, 01313-902, São Paulo, SP, Brazil.</institution>
    </aff>
  ...


.. note:: 
 * Do not include ``<xref>`` in ``<sup>``.

.. {"reviewed_on": "20180516", "by": "fabio.batalha@erudit.org"}