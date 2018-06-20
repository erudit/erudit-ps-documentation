.. _element-disp-formula:

<disp-formula>
==============

Mandatory attributes:

  1. ``@id`` (ver :ref:`id-attribution-tips`)

+----------------------------------------+--------------------+
| Appears in                             | Freqnency          |
+========================================+====================+
| :ref:`element-body`                    | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-p`                       | Zero or more times |
+----------------------------------------+--------------------+
| ``<th>``                               | Zero or more times |
+----------------------------------------+--------------------+
| ``<td>``                               | Zero or more times |
+----------------------------------------+--------------------+
| :ref:`element-supplementary-material`  | Zero or more times |
+----------------------------------------+--------------------+

Identifies equations and formulas displayed as blocks, it could be outside of a paragraph. The coding could be written according to :term:`W3C` using :term:`MathML` (http://www.w3.org/TR/MathML3/), or coded in Tex, LaTeX or even as an image using the element :ref:`element-graphic` as displayed in the examples.
 
Examples:

  * :ref:`element-dispmath-example-1`
  * :ref:`element-displatex-example-2`
  * :ref:`element-dispimg-example-3`

.. _element-dispmath-example-1:

Equation as MathML:
-------------------

.. code-block:: xml

    <!-- codificar: σˆ2 -->

    ...
    <xref ref-type="disp-formula" rid="e3">Equation 3</xref>
    ...
    <disp-formula id="e3">
      <mml:math id="m1" display="block">
        <mml:mrow>
          <mml:msub>
            <mml:mi>q</mml:mi>
            <mml:mi>c</mml:mi>
          </mml:msub>
          <mml:mo>=</mml:mo>
          <mml:mi>h</mml:mi>
          <mml:mrow>
            <mml:mo>(</mml:mo>
            <mml:mrow>
              <mml:mi>T</mml:mi>
              <mml:mo>−</mml:mo>
              <mml:msub>
                <mml:mi>T</mml:mi>
                <mml:mn>0</mml:mn>
              </mml:msub>
            </mml:mrow>
            <mml:mo>)</mml:mo>
          </mml:mrow>
        </mml:mrow>
     </mml:math>
     <label>(3)</label>
    </disp-formula>
    ...

.. _element-displatex-example-2:

Equation as LaTeX:
------------------

.. code-block:: xml

    ...
    <disp-formula id="e10">
        <label>(1)</label>
        <tex-math id="tx1">
            \documentclass {article}
            \usepackage{wasysym}
            \usepackage[substack]{amsmath}
            \usepackage{amsfonts}
            \usepackage{amssymb}
            \usepackage{amsbsy}
            \usepackage[mathscr]{eucal}
            \usepackage{mathrsfs}                           
            \usepackage{pmc}
            \usepackage[Euler]{upgreek}
            \pagestyle{empty}
            \oddsidemargin -1.0in
            \begin{document}
            \[E_it=α_i+Z_it γ+W_it δ+C_it θ+∑_i^n EFind_i+∑_t^n EFtemp_t+ ε_it                                 \]
            \end{document}
        </tex-math>
    </disp-formula>
    ...

.. _element-dispimg-example-3:

Equation as imagem:
-------------------

.. code-block:: xml

    ...
    <p>The Eh measurements were recalculated to the standard hydrogen potential (Standard Hydrogen Electrode - SHE), using the following <xref ref-type="disp-formula" rid="e1">equation 1</xref>(in mV):</p>
    <disp-formula id="e1">
        <graphic xlink:href="1234-5678-rctb-45-05-0110-e01.tif"/>
    </disp-formula>
    ...

.. {"reviewed_on": "20180620", "by": "fabio.batalha@erudit.org"}