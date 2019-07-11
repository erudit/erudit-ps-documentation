.. _element-disp-quote:

<disp-quote>
============

+----------------------+--------------------+
| Appears in           | Frequency          |
+======================+====================+
| :ref:`element-body`  | Zero or more times |
+----------------------+--------------------+
| :ref:`element-p`     | Zero or more times |
+----------------------+--------------------+
| :ref:`element-sec`   | Zero or more times |
+----------------------+--------------------+

Describes a citation from another source. Generally, this information is displayed in a document with indentation, more than three lines and a different font size to highlight it in the document.

For the ``@content-type`` attribute the allowed values are:

* verbatim
* dedication
* epigraph
* example
* block-citation

Examples:

    * :ref:`element-disp-quote-example-1`
    * :ref:`element-disp-quote-example-2`
    * :ref:`element-disp-quote-example-3`
    * :ref:`element-disp-quote-example-4`
    * :ref:`element-disp-quote-example-5`
    * :ref:`element-disp-quote-example-6`

.. _element-disp-quote-example-1:

Exemple of ``<disp-quote>`` for verbarim:
-----------------------------------------

.. code-block:: xml

    <disp-quote content-type="verbatim">
        <p>We suppose (i) that a priori judgement will play a part in the operation of any coherent system of belief, and (ii) that non-cognitivism about necessity had probably better grant a role for judgements of necessity as co-ordinate to (some) a priori judgements. If supposition (i) is wrong, then global Caution about necessitated judgements is, after all, at the service of the non-cognitivist about necessity</p>
    </disp-quote>

.. _element-disp-quote-example-2:

Exemple of ``<disp-quote>`` for epigraph:
-----------------------------------------

.. code-block:: xml

    <disp-quote content-type="epigraph">
        <p>La voie d’accès au présent a nécessairement la forme d’une archéologie.</p>
        <attrib>Giorgio Agamben, <italic>Qu’est-ce que le contemporain ?</italic></attrib>
    </disp-quote>


.. _element-disp-quote-example-3:

Exemple of ``<disp-quote>`` for dedication:
-------------------------------------------

.. code-block:: xml

    <disp-quote content-type="dedication">
        <p>En souvenir de Catherine Viollet</p>
    </disp-quote>

.. _element-disp-quote-example-4:

Exemple of ``<disp-quote>`` for example:
----------------------------------------

.. code-block:: xml

    <disp-quote content-type="dedication">
        <p>En souvenir de Catherine Viollet</p>
    </disp-quote>

.. _element-disp-quote-example-5:

Exemple of ``<disp-quote>`` for block-citation:
-----------------------------------------------

.. code-block:: xml

    <disp-quote content-type="dedication">
        <p>En souvenir de Catherine Viollet</p>
    </disp-quote>

.. _element-disp-quote-example-6:

Exemple of general ``<disp-quote>``:
------------------------------------

.. code-block:: xml

    <p>In the face of the failure of the transmission argument Wright would, apparently, endorse the view that Caution could still provide an adequate route to an anti-realist account of necessity, as can be gathered from the following passage:</p>
    <p>
        <disp-quote>
            <p>We suppose (i) that a priori judgement will play a part in the operation of any coherent system of belief, and (ii) that non-cognitivism about necessity had probably better grant a role for judgements of necessity as co-ordinate to (some) a priori judgements. If supposition (i) is wrong, then global Caution about necessitated judgements is, after all, at the service of the non-cognitivist about necessity</p>
        </disp-quote>
    </p>
    <p>I disagree. In the previous section we saw that showing that Caution is an incoherent attitude is not an easy matter.</p>


.. {"reviewed_on": "20190711", "by": "fabio.batalha@erudit.org"}
