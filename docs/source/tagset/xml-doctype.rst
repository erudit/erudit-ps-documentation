.. _xml-doctype:

<!DOCTYPE>
==========

The ``<!DOCTYPE>`` declaration indicates the :term:`DTD` to which the :term:`XML` is associated, i other words, it defines the rules for the structure of the :term:`document`. the :term:`Érudit Publishing Schema` is based on the JATS version `1.1 <http://jats.nlm.nih.gov/publishing/1.1/>`_.

Example *JATS version 1.1*:

.. code-block:: xml

    <!DOCTYPE article PUBLIC "-//NLM//DTD JATS (Z39.96) Journal Publishing DTD v1.1 20151215//EN" "https://jats.nlm.nih.gov/publishing/1.1/JATS-journalpublishing1.dtd">


Floating Elements
=================

Floating elements can appear anywhere in the :term:`document`, be it in :ref:`element-article` :ref:`element-sub-article` or in :ref:`element-response` in the blocks: :ref:`element-article-meta`, :ref:`element-body` and :ref:`element-back`.


Examples:

  * :ref:`elemento-xrefflut-example-1`
  * :ref:`elemento-xrefflut-example-2`
  * :ref:`elemento-xrefflut-example-3`


.. _elemento-xrefflut-example-1:

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


.. _elemento-xrefflut-example-2:

Example of floating element ``<xref>`` in ``<p>``:
--------------------------------------------------

.. code-block:: xml

    ...
    <body>
        <p>text text text text text text text (<xref ref-type="bibr" rid="B42">Da Silva, 1976</xref>). text text text</p>
    ...
    </body>
    ...


.. _elemento-xrefflut-example-3:

Example of floaring element ``<xref>`` in elements of ``<back>``:
-----------------------------------------------------------------

.. code-block:: xml

    ...
    <fn fn-type="other" id="fn2">
        <label>1</label>
            <p>Compreende-se por habilidades "comportamentos ou conjuntos de comportamentos que caracterizam determinado desempenho do indivíduo" (<xref ref-type="bibr" rid="B22">Santos, Kienen, Viecili, Botomé, &amp; Kubo, 2009</xref>, p. 133-134).</p>
    </fn>
    ...




.. {"reviewed_on": "20180422", "by": "fabio.batalha@erudit.org"}
