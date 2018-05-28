.. _element-p:

<p>
===


+--------------------------------+-------------------+
| Appears in                     | Frequency         |
+================================+===================+
| :ref:`element-abstract`        | One or more times |
+--------------------------------+-------------------+
| :ref:`element-ack`             | One or more times |
+--------------------------------+-------------------+
| :ref:`element-app`             | One or more times |
+--------------------------------+-------------------+
| :ref:`element-body`            | One or more times |
+--------------------------------+-------------------+
| :ref:`element-boxed-text`      | One or more times |
+--------------------------------+-------------------+
| ``<def>``                      | One or more times |
+--------------------------------+-------------------+
| :ref:`element-disp-quote`      | One or more times |
+--------------------------------+-------------------+
| :ref:`element-fn`              | One or more times |
+--------------------------------+-------------------+
| ``<list-item>``                | One or more times |
+--------------------------------+-------------------+
| :ref:`element-ref-list`        | One or more times |
+--------------------------------+-------------------+
| :ref:`element-sec`             | One or more times |
+--------------------------------+-------------------+
| :ref:`element-trans-abstract`  | One or more times |
+--------------------------------+-------------------+

Element which identifies a paragraph of text. It must be inserted in the :term:`document` without any attribute.

Example:

.. code-block:: xml

   ...
   <boxed-text id="box1">
     <sec>
       <title>Box 1. De Humanis corporis fabrica libri septem, or the <italic>Fabrica</italic>, and others.</title>
       <p><italic>De humani corporis fabrica libri septem,  </italic> the <italic>Fabrica</italic>,1<sup>st  </sup>edition, came to light in 1543, by the printer Johannes Oporinus, from Basel. It is one of the most influential books on human anatomy, and considered one of the great scientific and artistic oeuvre of mankind. The <italic>Fabrica</italic> is illustrated with detailed illustrations, printed with woodcut engravings, in Venice, with the identity of the artist is uncertain.</p>
       <p>The <italic>Fabrica,</italic> 2<sup>nd</sup> edition, released in 1555, dedicated to Charles V, is considered more sumptuous than the 1<sup>st  </sup>one. There are also corrections, decrease of redundancies, as well as inclusion of physiological experiments, by means of nervous section, e.g., section of the recurrent nerve, with consequent laryngeal paralysis.</p>
       <p><italic>De Humani corporis fabrica librorum Epitome</italic>, the <italic>Epitome</italic>, printed in 1543, was intended by Vesalius to be a very brief descriptive book, being a remarkable condensation of the 1<sup>st</sup> edition of the main book. It has 6 chapters, the 5<sup>th</sup> concerned with "The brain and the nervous system".  </p>
     </sec>
   </boxed-text>
   ...

.. {"reviewed_on": "20180528", "by": "fabio.batalha@erudit.oth"}