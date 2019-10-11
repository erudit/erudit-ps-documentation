.. _xml-doctype:

<!DOCTYPE>
==========

The ``<!DOCTYPE>`` declaration indicates the :term:`DTD` to which the :term:`XML` is associated, in other words, it defines the rules for the structure of the :term:`document`. the :term:`Érudit Publishing Schema` is based on the :term:`NISO JATS Journal Archiving DTD`.

Example (this example may not be up to date) *JATS version 1.2*:

.. code-block:: xml

    <!DOCTYPE article PUBLIC "-//NLM//DTD JATS (Z39.96) Journal Archiving and Interchange DTD v1.2 20190208//EN" "https://jats.nlm.nih.gov/archiving/1.2/JATS-archivearticle1.dtd">


Floating Elements
=================

Floating elements can appear anywhere in the :term:`document`, be it in :ref:`element-article` :ref:`element-sub-article` or in :ref:`element-response` in the blocks: :ref:`element-article-meta`, :ref:`element-body` and :ref:`element-back`.


Examples:

  * :ref:`element-xrefflut-example-1`
  * :ref:`element-xrefflut-example-2`
  * :ref:`element-xrefflut-example-3`


.. _element-xrefflut-example-1:

Example of floating element ``<xref>`` in ``<article-meta>``:
-------------------------------------------------------------

.. code-block:: xml

    ...
    <article-meta>
        ...
        <contrib contrib-type="author">
            <name>
                <surname>
                <given-names>
            </name>
            <xref ref-type="aff" rid="aff01">1</xref>
        </contrib>
    ...
    </article-meta>
    ...


.. _element-xrefflut-example-2:

Example of floating element ``<xref>`` in ``<p>``:
--------------------------------------------------

.. code-block:: xml

    ...
    <body>
        <p>text text text text text text text (<xref ref-type="bibr" rid="B42">Da Silva, 1976</xref>). text text text</p>
    ...
    </body>
    ...


.. _element-xrefflut-example-3:

Example of floaring element ``<xref>`` in elements of ``<back>``:
-----------------------------------------------------------------

.. code-block:: xml

    ...
    <fn fn-type="other" id="fn2">
        <label>1</label>
            <p>Compreende-se por habilidades "comportamentos ou conjuntos de comportamentos que caracterizam determinado desempenho do indivíduo" (<xref ref-type="bibr" rid="B22">Santos, Kienen, Viecili, Botomé, &amp; Kubo, 2009</xref>, p. 133-134).</p>
    </fn>
    ...




.. {"reviewed_on": "2019-10-11", "by": "mathieu.pigeon@erudit.org"}
