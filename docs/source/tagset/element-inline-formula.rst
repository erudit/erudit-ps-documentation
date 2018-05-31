.. _element-inline-formula:

<inline-formula>
================

+-------------------------+--------------------+
| Appears in              | Frequency          |
+=========================+====================+
| :ref:`element-p`        | Zero or more times |
+-------------------------+--------------------+
| :ref:`element-sec`      | Zero or more times |
+-------------------------+--------------------+
| ``th``                  | Zero or more times |
+-------------------------+--------------------+
| ``td``                  | Zero or more times |
+-------------------------+--------------------+

Used to identify equations encoded inline with the text. In such cases, the encoding may be in the :term:`W3C MathML` encoding standard where the base element is ``<mml:math>``, or in other encoding standards such as ASCII, TeX or LaTeX.

Identifica equações e fórmulas exibidas em um parágrafo. A codificação pode ser escrita de acordo com :term:`W3C` em linguagem :term:`MathML` (http://www.w3.org/TR/MathML3/), sendo o elemento base ``<mml:math>`` ou com codificação TeX ou LaTeX.

Example to code σˆ2* using *MathML*:

.. code-block:: xml

    ...
    <p>Nulla velit magna, semper quis dignissim id, condimentum nec diam
    <inline-formula>
        <mml:math id="e03">
            <mml:mrow>
                <mml:msup>
                    <mml:mover accent="true">
                        <mml:mi>σ</mml:mi>
                        <mml:mo>ˆ</mml:mo>
                    </mml:mover>
                    <mml:mn>2</mml:mn>
                </mml:msup>
            </mml:mrow>
        </mml:math>
    </inline-formula>
    Nulla quis leo sed turpis congue finibus feugiat ut dui. Donec id tincidunt tellus. Nunc fermentum dolor et congue convallis. <p/>
    ...

.. {"reviewed_on": "20180531", "by": "fabio.batalha@erudit.org"}
