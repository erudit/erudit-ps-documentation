.. _element-inline-graphic:

<inline-graphic>
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

Used to identify items inserted as inline images anchored in a paragraph. It could b used to represent some special character as image or a small formula that fits in text line as image.

.. note:: 

  For formulas written in mathml see the element :ref:`element-inline-formula`


Example:

.. code-block:: xml

  ...
  <p>We also used an enrichment factor for surface waters (EF<sub>w</sub>) based on the equation:<inline-graphic xlink:href="image.tif"/>. The EF<sub>s</sub> and EF<sub>w</sub> quantified the concentration of the element of interest (C<sub>i</sub>) in the sample, in relation to the (natural) geochemical background.</p>
  ...


.. {"reviewed_on": "20180531", "by": "fabio.batalha@erudit.org"}
